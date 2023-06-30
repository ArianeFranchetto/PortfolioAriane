<template>

    <div class='navbar-fixed-bottom' id="footer">
    
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
    margin-top: 5px;
}



img:hover {
    width: 50px;
    margin-top: 5px;
}

#footer {
    display: flex;
    flex-direction: row;
align-items: center;
justify-content: space-around;

padding: 6px;
width: 100%;
   position: fixed;
    bottom:0;
    background-image: linear-gradient(10deg, #fddeea 0, #f2d1e1 16.67%, #e2bdd4 33.33%, #cca4c3 50%, #b48cb4 66.67%, #a07baa 83.33%, #8f71a5 100%);
    


 
}

@media (max-width: 750px) {
    img {
        width: 35px;
        display: flex;
        flex-wrap: wrap;
        flex-direction: column;
        margin-right: 10px;
    }

    img:hover {
        width: 40px;
    }

    .footer {
        display: flex;
        flex-direction: row;
       
       
    }

}


@media ( max-width: 600px ) {
    img {
        width: 35px;
        display: flex;
        flex-wrap: wrap;
        flex-direction: column;
        margin-right: 10px;
    }

    img:hover {
        width: 40px;
    }

    .footer {
        display: flex;
        flex-direction: row;
       
       
    }


}

</style>