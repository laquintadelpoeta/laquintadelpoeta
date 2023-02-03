<script setup>
import { ref } from 'vue'

const categories = ref([
    {name: 'Malo', key: 1}, 
    {name: 'Regular', key: 2}, 
    {name: 'Medio', key: 3}, 
    {name: 'Bueno', key: 4},
    {name: 'Excelente', key: 5}
])
const nombre = ref()
const trato = ref()
const limpieza = ref()
const comodidad = ref()
const instalaciones = ref()
const decoracion = ref()
const relacion = ref()
const resultado = ref()
const opiniones = ref()
const email = ref()
</script>

<template>
    <div>
        <div class="flex justify-content-center">
            <Card>
                <template #title>
                    Cuestionario de satisfacción
                </template>
                <template #content>
                    <div class="flex">
                        <span>Nombre</span>
                        <InputText type="text" v-model="nombre" />
                    </div>
                    <div v-for="category of categories.slice().reverse()" :key="category.key" class="field-radiobutton inline mr-3">
                        <RadioButton :inputId="category.key" name="category" :value="category.name" v-model="trato" />
                        <label :for="category.key">{{category.name}}</label>
                    </div>
                    <br>
                    <div v-for="category of categories.slice().reverse()" :key="category.key" class="field-radiobutton inline mr-3">
                        <RadioButton :inputId="category.key" name="category" :value="category.name" v-model="trato" />
                        <label :for="category.key">{{category.name}}</label>
                    </div>
                    <br>
                    <div v-for="category of categories.slice().reverse()" :key="category.key" class="field-radiobutton inline mr-3">
                        <RadioButton :inputId="category.key" name="category" :value="category.name" v-model="trato" />
                        <label :for="category.key">{{category.name}}</label>
                    </div>
                    <br>
                    <div v-for="category of categories.slice().reverse()" :key="category.key" class="field-radiobutton inline mr-3">
                        <RadioButton :inputId="category.key" name="category" :value="category.name" v-model="trato" />
                        <label :for="category.key">{{category.name}}</label>
                    </div>
                    <br>
                    <div v-for="category of categories.slice().reverse()" :key="category.key" class="field-radiobutton inline mr-3">
                        <RadioButton :inputId="category.key" name="category" :value="category.name" v-model="trato" />
                        <label :for="category.key">{{category.name}}</label>
                    </div>
                    <br>
                    <div v-for="category of categories.slice().reverse()" :key="category.key" class="field-radiobutton inline mr-3">
                        <RadioButton :inputId="category.key" name="category" :value="category.name" v-model="trato" />
                        <label :for="category.key">{{category.name}}</label>
                    </div>
                    <br>
                    <div v-for="category of categories.slice().reverse()" :key="category.key" class="field-radiobutton inline mr-3">
                        <RadioButton :inputId="category.key" name="category" :value="category.name" v-model="trato" />
                        <label :for="category.key">{{category.name}}</label>
                    </div>
                    <br>
                    <div v-for="category of categories.slice().reverse()" :key="category.key" class="field-radiobutton inline mr-3">
                        <RadioButton :inputId="category.key" name="category" :value="category.name" v-model="trato" />
                        <label :for="category.key">{{category.name}}</label>
                    </div>
                </template>
            </Card>
        </div>
    </div>
</template>
