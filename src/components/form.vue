<template>
<div class="wrapper">
    <div class="left">
        <h3>
            send a message
        </h3>
        <h1>
            Get in <span>Touch</span>
        </h1>
        <p>
            We will respond to your message as soon as possible.
        </p>
            <form>
                <input type="text" id="fname" name="fname" placeholder="Name">
                <input type="email" id="email" name="email" placeholder="Email">
                <input type="tel" id="phone" name="phone" placeholder="Phone">
                <input type="info" id="info" name="info" placeholder="More Info">
                <textarea name="text" id="text" cols="50" rows="10"></textarea>
                <input type="submit" placeholder="Send">
            </form> 
    </div>
    <div class="right">

    </div>
</div>
</template>

<script>
export default {
    name:'Form',

}
</script>

<style lang="scss" scoped>
    .message {
        height: 200px;
        width: 300px;
    }
</style>