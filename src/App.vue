<script setup>
import ParentComponent from "./components/bai1/ParentComponent.vue";
// import ProductChildren from "./components/bai2/ProductChildren.vue";
import ProductParent from "./components/bai2/ProductParent.vue";
import BaseButton from "./components/BaseButton.vue";
import SlotComponent from "./components/SlotComponent.vue";
import CountParent from "./components/bai3/CountParent.vue";
import TodoApp from "./components/bai4/TodoApp.vue";
import Modal from "./components/bai5/Modal.vue";
import App from "./components/bai5/App.vue";
import Card from "./components/bai6/Card.vue";
</script>

<template>
  <div>
    <SlotComponent>
      <!------noi dung nay se chinh la slot s-->
      <a href="">Facebook</a>
    </SlotComponent>
    <ParentComponent />
    <BaseButton>
      <a href="">click me</a>
    </BaseButton>
    <!-- <BaseButton title="add product" /> -->
  
     <ProductParent/>
     <CountParent></CountParent>
     <TodoApp></TodoApp><br>
     <Modal></Modal>
     <App></App>
     <Card>
      <template #header>Thông báo từ hệ thống</template>
      <template #body>Thông báo từ hệ thống</template>
      <template #footer>Thông báo từ hệ thống</template>
     </Card>
  </div>
</template>

<style></style>
