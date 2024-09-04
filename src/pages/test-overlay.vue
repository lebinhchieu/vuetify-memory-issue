<template>
  <div>
    Hi, I am overlay {{ testObject.testVar[0] }}
    <VBtn to="/" text="Back to home"></VBtn>
    <VBtn text="Open overlay">
      <VOverlay activator="parent">
        <VCard title="Overlay title">
          <VCardText>
            I am overlay body
          </VCardText>
        </VCard>
      </VOverlay>
    </VBtn>
  </div>
</template>

<script setup>
import { TestObject } from '../objects/test-object.js'

const testObject = new TestObject()
</script>
