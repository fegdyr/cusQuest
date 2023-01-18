<template>
    <h3>Question {{ question.number }} </h3>
    <p>{{ question.text }}</p>
    <li v-for="(option, index) in question.answerOptions">
        <button value="{{ index }}">option</button>
    </li>
</template>

<script>
export default {
    data() {
        return {
            question: {
                number: 3,
                text: "How many bolts do the bridge to Öland have?",
                answerOptions: [
                    "2000",
                    "20000",
                    "200000",
                    "2000000",
                    "20000000"
                ],
                answerIndex: 3
            }
        }
    },
}
</script>