<template>
  <div class="avaliations">

        <section class="classification">
            <div v-for="(student, index) in Alunos" :key="index" class="student-avaliation">
                    <p> <i class="bi bi-star-fill"></i>
                        <i class="bi bi-star-fill"></i>
                        <i class="bi bi-star-fill"></i>
                        <i class="bi bi-star-fill"></i>
                        <i class="bi bi-star"></i>
                        (4.0)
                    </p>

                <p class="text-avaliation student">{{ student.avaliation }}</p>

                <h5 class="name-student">{{ student.name }}</h5>
            </div>
        </section>
    </div>
</template>

<script>
export default {

    data(){
        return{
            Alunos:[
                {
                    name: 'Maria A.',
                    avaliation: '"A Professora Juliana é incrível! Ela tornou a matemática divertida e me ajudou a melhorar minhas notas."',
                },
                {
                    name: 'João S.',
                    avaliation: '"Aprendi mais com a Professora Juliana em um mês do que em um ano na escola."',
                }
            ]
        }
    }
}
</script>

<style>
.avalations{

    display: flex;
}
.classification{

    width: 100%;
    margin: 0px 75px;
}
.student-avaliation{

    display: inline-flex;
    width: 450px;
    padding: 32px;
    flex-direction: column;
    align-items: flex-start;
    gap: 32px;
    border-radius: 8px;
    border: 1px solid #D9D9D9;
    margin: 0px 20px;
}
.student-avaliation i{

    color: orange;
    padding: 0px 2px;
}
.text-avaliation.student{
    color: #5C5C5C;
    font-family: Helvetica Neue;
    font-size: 20px;
    font-style: italic;
    font-weight: 400;
    line-height: 150%; /* 30px */
    align-self: stretch;
}
.name-student{
    align-self: stretch;
    color: #1E1E1E;
    font-family: Helvetica Neue;
    font-size: 20px;
    font-style: normal;
    font-weight: 500;
    line-height: 150%; /* 30px */
}
</style>