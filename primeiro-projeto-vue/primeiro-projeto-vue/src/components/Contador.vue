<template>
	<div>
		<p>Contador:</p>
		<div id="number">{{ number }}</div>
		<button @click="add">+</button>
		<button @click="sub">-</button>
	</div>
</template>

<script>
export default {
	name: 'Contador-exercise',
	data() {
		return {
			number: 0
		}
	},
	methods: {
		add() {
			this.number = this.number + 1;
		},
		sub() {
			this.number = this.number - 1;
		}
	}
}
</script>

// let add = document.getElementById('add');
// let sub = document.getElementById('sub');
// let number = document.getElementById('number');
// let integer = 0;

// add.addEventListener('click', function() {
// 	integer += 1;
// 	number.innerHTML = integer;

// });

// sub.addEventListener('click', function() {
// 	integer -= 1;
// 	number.innerHTML = integer;
// });