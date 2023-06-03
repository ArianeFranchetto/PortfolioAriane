<template>
    <div class="footer">
        <a href="https://github.com/ArianeFranchetto"><img src="../assets/img/github.png" alt="img-github"></a>
        <a href="https://www.linkedin.com/in/ariane-franchetto/"><img src="../assets/img/linkedin.png" alt="img-linkedin"></a>
        <a href="file:///C:/Users/caiop/Downloads/ArianeCurriculo.pdf"><img src="../assets/img/curriculo.png" alt="img-curriculo"></a>
    </div>
</template>
<script>
export default {

}
</script>

<style scoped>
img {
    width: 60px;
    box-shadow: 12px 13px 31px 8px rgba(0,0,0,0.75);
    border-radius: 100px;
}



img:hover {
    width: 50px;
}

.footer {
    display: flex;
    justify-content: center;
    justify-content: space-around;
    margin-top: 50px;
 
}

@media ( max-width: 600px ) {
    img {
        width: 50px;
        display: flex;
        flex-wrap: wrap;
        flex-direction: column;
    }

    img:hover {
        width: 40px;
    }
}

</style>