<template>
  <div class="faq-container">
    <h1 class="faq-heading">FAQ</h1>
    <div class="faq-list">
      <div v-for="(question, index) in faqData" :key="index" class="faq-item">
        <div class="question-wrapper">
          <h3 class="question">{{ question.question }}</h3>
          <span class="dropdown-arrow" @click="toggleAnswer(index)">
            &#9662;
          </span>
        </div>
        <div v-if="selectedQuestion === index" class="answer">
          {{ question.answers }}
        </div>
      </div>
    </div>
  </div>
</template>
  
  <script>
export default {
  data() {
    return {
      faqData: [
        {
          question: "Question here Lorem ipsum?",
          answers:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        },
        {
          question: "Lorem ipsum dolor sit amet, consectetur adipiscing elit",
          answers:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        },
        {
          question: "Lorem ipsum dolor sit amet, consectetur adipiscing elit",
          answers:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        },
        {
          question: "Lorem ipsum dolor sit amet, consectetur adipiscing elit",
          answers:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        },
        // Add more questions and answers as needed
      ],
      selectedQuestion: null,
      selectedAnswerIndex: null,
    };
  },
  methods: {
    toggleAnswer(index) {
      if (this.selectedQuestion === index) {
        this.selectedQuestion = null;
        this.selectedAnswerIndex = null;
      } else {
        this.selectedQuestion = index;
        this.selectedAnswerIndex = 0; // Default to first answer
      }
    },
  },
};
</script>
  <style>
.faq-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 429px;
  /* width: 710px; */
  text-align: center;
  /* gap: 1000px; */
  justify-content: space-evenly;
}

.faq-heading {
  font-size: 24px;
  margin-bottom: 20px;
  color: #001D3D;
}

.faq-item {
  margin-bottom: 20px;
  padding-bottom: 20px; /* Add padding at the bottom of each item for the line */
  border-bottom: 1px solid #ccc; /* Add a border at the bottom to create the line */
}
.faq-item:last-child {
  border-bottom: none; /* Remove the border from the last question item */
}

.question-wrapper {
  display: flex;
  align-items: center;
  justify-content: space-between;
  cursor: pointer;
  width: 710px;
}

.question {
  margin: 0;
  color: 
#001D3D;
}

.dropdown-arrow {
  font-size: 20px;
  margin-left: 10px; /* Adjust this value as needed */
}

.answer {
    margin-top: 10px;
    width: 708px;
    color: #001D3D;
}
</style>