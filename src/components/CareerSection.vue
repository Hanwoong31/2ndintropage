<template>
  <section id="career" class="career-section">
    <h2 class="section-title">나의 경력</h2>
    <div class="card-grid">
      <div
        class="card"
        v-for="(item, index) in careers"
        :key="index"
      >
        <div class="icon">{{ item.icon }}</div>
        <h3 class="card-title">{{ item.title }}</h3>
        <p class="card-description">{{ item.description }}</p>
      </div>
    </div>
  </section>
</template>

<script setup>
const careers = [
  {
    icon: '🎵',
    title: '음악 창작자 (힙합 & 뮤지컬)',
    description:
      '감정과 사유를 음악으로 표현합니다. 로직 프로와 AI 툴을 활용해 창작 중입니다.',
  },
  {
    icon: '📝',
    title: '광고 기획자 & 카피라이터',
    description:
      '브랜드 캠페인을 기획하고, 감성을 담은 카피로 메시지를 전달하는 일을 해왔습니다.',
  },
  {
    icon: '📐',
    title: '수학 & 영어 강사',
    description:
      '학생들과 논리와 언어의 아름다움을 나누며 가르친 경험이 있습니다.',
  },
  {
    icon: '🧠',
    title: '심리학, 뇌과학, 철학 탐구자',
    description:
      '인간의 마음과 존재를 탐구하고 창작에 연결하려는 시도를 계속하고 있습니다.',
  },
]
</script>

<style scoped>
.career-section {
  padding: 4rem 1rem;
  background-color: #f9f9f9;
  text-align: center;
}

.section-title {
  font-size: 2.2rem;
  font-weight: bold;
  margin-bottom: 2.5rem;
}

.card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
  max-width: 1000px;
  margin: 0 auto;
}

.card {
  background: white;
  border-radius: 1.2rem;
  padding: 2rem;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.05);
  transition: transform 0.2s ease;
}

.card:hover {
  transform: translateY(-5px);
}

.icon {
  font-size: 2.8rem;
  margin-bottom: 1rem;
}

.card-title {
  font-size: 1.3rem;
  font-weight: 600;
  margin-bottom: 0.6rem;
}

.card-description {
  font-size: 1rem;
  color: #555;
  line-height: 1.6;
}
</style>
