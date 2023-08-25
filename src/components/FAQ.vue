<template>
  <div class="faq-container">
    <h1 class="faq-heading">FAQ</h1>
    <div class="faq-list">
      <div
        v-for="(question, index) in faqData"
        :key="index"
        class="faq-item"
        :class="{ 'open': selectedQuestion === index }"
      >
        <div class="question-wrapper" @click="toggleAnswer(index)">
          <h3 class="question">{{ question.question }}</h3>
          <span class="dropdown-arrow">&#9662;</span>
        </div>
        <div v-if="selectedQuestion === index" class="answer">{{ question.answers }}</div>
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
    };
  },
  methods: {
    toggleAnswer(index) {
      if (this.selectedQuestion === index) {
        this.selectedQuestion = null;
      } else {
        this.selectedQuestion = index;
      }
    },
  },
};
</script>

<style>
.faq-container {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
}

.faq-heading {
  font-size: 24px;
  margin-bottom: 20px;
  color: #001d3d;
  text-align: center;
}

.faq-item {
  margin-bottom: 20px;
  border-bottom: 1px solid #ccc;
  padding-bottom: 10px;
  transition: max-height 0.3s ease-out;
  max-height: 50px;
  overflow: hidden;
}

.faq-item.open {
  max-height: 300px;
}

.question-wrapper {
  display: flex;
  align-items: center;
  cursor: pointer;
}

.question {
  margin: 0;
  color: #001d3d;
  flex-grow: 1;
}

.dropdown-arrow {
  font-size: 20px;
}

.answer {
  margin-top: 10px;
  color: #001d3d;
}
</style>
