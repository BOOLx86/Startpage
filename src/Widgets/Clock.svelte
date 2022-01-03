<script>
    let time = '00:00';

    get_time();
    setInterval(get_time, 1000);

    function get_time() {
        var date = new Date();
        time = date.getHours() + ':' + ('0' + date.getMinutes()).slice(-2);
    }
</script>


<div id="clock"> {time} </div>

<style>
    #clock {
        font-size: 10em;
        font-weight: bold;
    }
    
</style>
