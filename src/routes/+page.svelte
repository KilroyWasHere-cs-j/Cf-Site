<script lang="ts">
    import Header from '../lib/Header.svelte';
    import Box from '../lib/Box.svelte';
	import YearBreak from '$lib/YearBreak.svelte';
	import PageEnder from '$lib/PageEnder.svelte';
	import Buffer from '$lib/Buffer.svelte';
	import Paragraph from '$lib/Paragraph.svelte';
	import PageHeader from '../lib/PageHeader.svelte';

	const rows = 8;
	const cols = 9;
	const w = 160;
	const h = 240;
	const src = 'https://media.istockphoto.com/id/174961182/photo/barbed-wire-fence.jpg?b=1&s=170667a&w=0&k=20&c=6F34YYklACxD-eFQfX1BLfh7Y_FkMgeKt1Tr0BFrAvY=';
	let current = 0;
</script>

<svelte:head>
	<title>Genocide Site</title>
	<style>
		body {
		  background: gray;
		}
	  </style>
</svelte:head>

<!--https://www.nytimes.com/interactive/2022/05/20/world/americas/enslaved-haiti-debt-timeline.html?unlocked_article_code=gbBkXR8Dvzax6Aa01PxdxbCTQq-VamFCGi05ArKVOONA4iTnd1dRu2B5Hcjdh0tG0OtN24QFYtC5VO2uqqqO3uaCqMpfUEQu08xCCrZ3vGqHJlJulDN2BAnwjRTzSw4-zYq5r0oS0uuFplQiOt12oMgbAun5EqbeR0THpQTGs7oPDA-OyayrutjQJKbTcpO2hfn2oV_SaTiM_TK02B8r6slCE0pkLbscRjoc50ru6pnT7ijxx8Tm2qWifCAcq5WGyOOPd3A2JUvYwuVSCb1ne62TKwtj5JNigHdsaqW4_gy5CKE44-NBTvWoe5tk3W_S9PpRcU5eBxKC0qnrguleu4zdF0yUvW3_V0y56Sv-ElsAs8piSVRIJlUQLTGp&smid=url-share-->


<div class="bg-cover" style="background-image: url({src}); height: 880px">
	<PageHeader header="Effect of war on genocide" subheader="September 1, 1939 – September 2, 1945" subtext="Gabriel Tower"/>
	<Box width=100 height=100 imagePath="https://images.unsplash.com/photo-1600267188229-1dd3dd776737?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8N3x8d29ybGQlMjB3YXIlMjAyfGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60"/>
	<Buffer width=100 height=100/>
	<Buffer width=100 height=100/>
	<YearBreak year="War start"/>
	<Box width=100 height=600>
		<Paragraph text="1933 Adolf Hitler came to power. During the years between 1933 - 1939, the Nazi party worked on laying the ground work for the percicution of Jews, Homosexuals, Roma, and many other groups."/>
		<Paragraph text="These laws allowed/promoted the boycott of jewish businesses, Evian confrence, Kristallnact, and forced emigration."/>
		<div class="w-24 h-1 bg-gray-500 mt-4"/>
		<Paragraph text="On September 1, 1939, Hitler invaded Poland from the west; two days later, France and Britain declared war on Germany, beginning World War II."/>
		<Paragraph text="The war did not stop the percicution. It made it worse."/>
	</Box>
	<YearBreak year=1939/>
	<Box width=100 height=600>
		<Header header="Germany annexes Czechoslovakia"/>
		<Header header="ST. Louis sails"/>
	</Box>
	<YearBreak year=1940/>
	<Box width=100 height=600>
		<Header header="Germany invades Poland"/>
		<Header header="First prisoners arrive at Auschwitz"/>
	</Box>
	<YearBreak year=1941/>
	<Box width=100 height=600>
		<Header header="Mass Murder begin at chelmno"/>
		<Header header="Operation Reinhard"/>
	</Box>
	<YearBreak year=1942/>
	<Box width=100 height=600/>
	<YearBreak year=1943/>
	<Box width=100 height=600/>
	<YearBreak year=1944/>
	<Box width=100 height=600/>
	<YearBreak year=1945/>
	<Box width=100 height=200 header="War is over"/>
	<PageEnder/>
</div>
