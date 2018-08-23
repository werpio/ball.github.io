<style>
    .lawn {
        background: green;
        height: 150px;
        display: flex;
        justify-content: space-between;

    }

    .ball {
        width: 100px;
        height: 100px;
        background: brown;
        border-radius: 100%;
        align-self: flex-end;
        
    }
    .ball2 {
        width: 100px;
        height: 100px;
        background: yellow;
        border-radius: 100%;
        align-self: flex-end;
        display:flex;
        
    }


</style>


<div class="lawn">

    <div class="ball"></div>
    <div class="ball2"></div>

</div>


<script>
    var ball = document.querySelector('.ball');
    var ballPosition = 0;
    var ball2Position = 0;
    var velocity = 1;

    setInterval(function () {
        ballPosition = ballPosition + 1;
        

        update()
        render()
    }, 15)

    function update() {
       
        ballPosition = ballPosition + velocity;
        
    }

    function render() {

        ball.style.marginLeft = ballPosition + 'px'
        

    }


    
</script>
