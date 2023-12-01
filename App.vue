<script>
import L4T1 from './tasks/lection_4/L4T1.vue';
import L4T2 from './tasks/lection_4/L4T2.vue';
import L4T3 from './tasks/lection_4/L4T3.vue';
import L5T1 from './tasks/lection_5/L5T1.vue';
import L5T2 from './tasks/lection_5/L5T2.vue';
import L5T3 from './tasks/lection_5/L5T3.vue';
import l5t5 from './tasks/lection_5/l5t5.vue';
import l5t6 from './tasks/lection_5/l5t6.vue';
import l5t7 from './tasks/lection_5/l5t7.vue';
import l5t8 from './tasks/lection_5/l5t8.vue';
import l5t9 from './tasks/lection_5/l5t9.vue';
import l5t10 from './tasks/lection_5/l5t10.vue';
import l5t11 from './tasks/lection_5/l5t11.vue';
import l5t12 from './tasks/lection_5/l5t12.vue';
import l5t13 from './tasks/lection_5/l5t13.vue';
import l5t14 from './tasks/lection_5/l5t14.vue';
import l5t15 from './tasks/lection_5/l5t15.vue';
import Employee from './tasks/lection_6/Employee.vue';
import l6t3 from './tasks/lection_6/l6t3.vue';
import l6t4 from './tasks/lection_6/l6t4.vue';
import l6t5 from './tasks/lection_6/l6t5.vue';

export default {
    data() {
        return {
        
            visible: true,
            visible2: false,
            p1: true,
            p2: true,
            p3: true,
            p4: true,
            p5: true,
            p6: true,
            hide: function () {
                this.visible2 = false;
            },
            show: function () {
                this.visible2 = true;
            },
            clickB1: function () {
                this.p1 = !this.p1;
            },
            clickB2: function () {
                this.p2 = !this.p2;
            },
            clickB3: function () {
                this.p3 = !this.p3;
            },
            clickB4: function () {
                this.p4 = !this.p4;
            },
            clickB5: function () {
                this.p5 = !this.p5;
            },
            clickB6: function () {
                this.p6 = !this.p6;
            },
            day: 5,
            show6: true,
            clickshow6: function () {
                this.show6 = false;
            },
            show7: true,
            clickshow7: function () {
                this.show7 = !this.show7;
            },
            arr: [2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30],
            arr2: ['a', 'b', 'c'],
            addItemToArr: function () {
                this.arr2.push('new');
            },
            DeleteItemToArr: function () {
                this.arr2.shift();
            }
        };
    },
    components: {
      L4T1,
      L4T2,
      L4T3,
      L5T1,
      L5T2,
      L5T3,
      l5t5,
        l5t6,
        l5t7,
        l5t8,
        l5t9,
        l5t10,
        l5t11,
        l5t12,
        l5t13,
        l5t14,
        l5t15,
        Employee,
        l6t3,
        l6t4,
        l6t5,
    }
}
</script>

<template>
  <h1>Task 1</h1>
  <p v-if="visible">text1</p>
  <p v-if="!visible">text2</p> 


  <h1> Task 2</h1>

  <p v-if="visible2">Hello</p>
  <button @click="show">Show</button>
  <button @click="hide">Hide</button>

  <h1> Task 3</h1>

  <p v-if="p1">P1</p>
  <p v-if="p2">P2</p>
  <p v-if="p3">P3</p>

  <button @click="clickB1">B1</button>
  <button @click="clickB2">B2</button>
  <button @click="clickB3">B3</button>

  <h1>Task 4</h1>

  <p v-if="p4">P4</p>
  <p v-if="p5">P5</p>
  <p v-if="p6">P6</p>

  <button @click="clickB4">{{p4 ? 'hide' : 'show'}}</button>
  <button @click="clickB5">{{p5 ? 'hide' : 'show'}}</button>
  <button @click="clickB6">{{p6 ? 'hide' : 'show'}}</button>

  <h1>Task 5</h1>

  <p v-if="day === 1">Пн</p>
  <p v-if="day === 2">Вт</p>
  <p v-if="day === 3">Ср</p>
  <p v-if="day === 4">Чт</p>
  <p v-if="day === 5">Пт</p>
  <p v-if="day === 6">Су</p>
  <p v-if="day === 7">Вс</p>

  <h1>Task 6</h1>

  <p v-show="show6">HGG</p>
  <p v-show="show6">HGGdf</p>
  <p v-show="show6">HGGgb</p>

  <button @click="clickshow6">Hide</button>

  <h1> Task 7</h1>

  <p v-show="show7">HGGgb</p>
  <button @click="clickshow7">{{show7 ? 'Hide': 'Show'}}</button>

  <h1>Lecton 3</h1>

  <h1>task 1</h1>

  <p v-for="item in arr" :key="item">{{item}}</p>

  <h1>task 2</h1>

  <ul>
    <li v-for="item in arr2" :key="item">{{item}}</li>
    <button @click="addItemToArr">New Item</button>
  </ul>

  <h1> Task 3</h1>


  <ul>
    <li v-for="item in arr2" :key="item">{{item}}</li>
    <button @click="DeleteItemToArr">Delete Item</button>
  </ul>


  <h1>Lection 4</h1>
  
  <L4T1 />
  <L4T2 />
  <L4T3 />


  <h1>Lection 5</h1>

  <L5T1 />
  <L5T2 />
  <L5T3 />
  <l5t5 />
  <l5t6 />
  <l5t7 />
  <l5t8 />
  <l5t9 />
  <l5t10 />
  <l5t11 />
  <l5t12 />
  <l5t13 />
  <l5t14 />
  <l5t15 />
  <Employee name="jogn" sur="Gur" />
  <l6t3 :arg="['ru', 'it', 'vv']" />
  <l6t4 />
  <l6t5 />

</template>