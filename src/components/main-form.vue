<template>
    <div class="container">
        <mainTitle />
        <div class="name-holder">
            <div class="name-input-holder">
                <label for="">First Name</label>
                <input type="text">
            </div>
            <div class="name-input-holder">
                <label for="">Last Name</label>
                <input type="text">
            </div>
        </div>
        <div class="email-holder">
            <div class="email-input-holder">
                <label for="">Email Address</label>
                <input type="text">
            </div>
        </div>
        <div class="query-holder">
            <div class="query-input-holder">
                <input type="radio" id="one" value="One" />
                <label class="radio-label" for="one">General Enquiry</label>
            </div>

            <div class="query-input-holder">
                <input type="radio" id="two" value="Two" />
                <label class="radio-label" for="two">Support Request</label>
            </div>
        </div>
        <div class="message-holder">
            <textarea class="message-text-holder" name="" id=""></textarea>
        </div>
    </div>
    <div>

    </div>
</template>


<script setup lang="ts">
import mainTitle from './main-title.vue';
</script>


<style scoped>
.container {
    width: 40%;
    margin: 50px auto;
    background-color: rgb(226, 230, 233);
    border-radius: 18px;
}

input[type="text"] {
    display: block;
    background-color: rgb(226, 230, 233);
    border-radius: 5px;
    padding: 18px 0;
    width: 100%;

}



label {
    margin: 10px 10px;
    display: block;
}

.radio-label {
    display: inline;
}

.name-holder {
    padding: 20px;
    width: 90%;
    margin: 10px auto;
    display: flex;
    justify-content: space-around;
    align-items: center;

}

.name-input-holder {
    width: 40%;
}

.email-holder {
    padding: 20px;
    width: 90%;
    margin: 10px auto;

}

.email-input-holder {
    width: 90%;
    margin: 0 auto;
}

.query-holder {

    padding: 20px;
    width: 90%;
    margin: 10px auto;
    display: flex;
    justify-content: space-around;
    align-items: center;
}

.query-input-holder {
    border: 1px solid rgb(69, 69, 69);
    width: 40%;
    padding: 20px;
    border-radius: 5px;
}

.message-holder {
    width: 90%;
    margin: 20px auto;
}

.message-text-holder {
    background-color: rgb(226, 230, 233);
    border-radius: 5px;
    display: block;
    width: 90%;
    margin: 10px auto;
    padding: 50px 0;
}
</style>


<!-- import { Field, Form, ErrorMessage } from 'vee-validate';
import * as yup from 'yup';

const schema = yup.object({
    email: yup.string().email().required(),
    name: yup.string().required(),
});

function onSubmit(values : any) {
    alert(JSON.stringify(values, null, 2));
} -->

<!--
<div>
            <Form :validation-schema="schema" @submit="onSubmit">
                <Field name="email" type="email" />
                <ErrorMessage style="color: red;" name="email" as="div" />

                <Field name="name" />
                <ErrorMessage style="color: red;" name="name" as="div" />

                <button>Submit</button>
            </Form>
        </div> -->