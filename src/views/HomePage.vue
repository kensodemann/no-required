<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Blank</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Blank</ion-title>
        </ion-toolbar>
      </ion-header>

      <ion-list>
        <ion-item>
          <ion-input required label="Name"></ion-input>
        </ion-item>

        <ion-item>
          <ion-checkbox required :indeterminate="true">Vegan?</ion-checkbox>
        </ion-item>

        <ion-item>
          <input type="checkbox" required />
          <label for="scales">Vegan?</label>
        </ion-item>

        <ion-item>
          <ion-select required label="Favorite Fruit" label-placement="stacked">
            <ion-select-option value="apple">Apple</ion-select-option>
            <ion-select-option value="banana">Banana</ion-select-option>
            <ion-select-option value="orange">Orange</ion-select-option>
          </ion-select>
        </ion-item>

        <ion-item>
          <select required>
            <option value="apple">Apple</option>
            <option value="banana">Banana</option>
            <option value="orange">Orange</option>
          </select>
        </ion-item>

        <ion-item>
          <ion-radio-group required>
            <ion-radio value="grapes">Grapes</ion-radio><br />
            <ion-radio value="strawberries">Strawberries</ion-radio><br />
            <ion-radio value="pineapple">Pineapple</ion-radio><br />
            <ion-radio value="cherries">Cherries</ion-radio>
          </ion-radio-group>
        </ion-item>
      </ion-list>

    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonCheckbox, IonContent, IonHeader, IonInput, IonItem, IonList, IonPage, IonRadio, IonRadioGroup, IonSelect, IonSelectOption, IonTitle, IonToolbar } from '@ionic/vue';

</script>

<style scoped>
#container {
  text-align: center;

  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;

  color: #8c8c8c;

  margin: 0;
}

#container a {
  text-decoration: none;
}
</style>
