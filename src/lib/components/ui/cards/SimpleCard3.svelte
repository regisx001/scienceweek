<script>
	import { cn } from '$lib/utils.js';
	import CardContainer2 from './Container2.svelte';

	let card = {
		title: 'Be Happy',
		desc: 'Life is a shipwreck, but we must not forget to sing in the lifeboats.'
	};
	let className = '';
	export { className as class };
</script>

<CardContainer2>
	<slot></slot>
</CardContainer2>
