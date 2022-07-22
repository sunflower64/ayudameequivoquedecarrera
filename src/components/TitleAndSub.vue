<template>
    <div class="column is-one-third has-text-left py-5 mx-6">
        <h1 class="title"> {{ title }} </h1>
        <h2 class="subtitle"> {{ subtitle }} </h2>
    </div>
</template>
<script>
    export default{
        props: {
            title: String,
            subtitle: String,
        }
    }
</script>