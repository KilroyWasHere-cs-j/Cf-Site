<script lang="ts">
    import Header from '../lib/Header.svelte';
    import Box from '../lib/Box.svelte';
	import YearBreak from '$lib/YearBreak.svelte';
	import PageEnder from '$lib/PageEnder.svelte';
	import Buffer from '$lib/Buffer.svelte';
	import Paragraph from '$lib/Paragraph.svelte';
	import PageHeader from '../lib/PageHeader.svelte';
	import ImageBox from '../lib/ImageBox.svelte';

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

<!--! Background-->
<!--https://images.unsplash.com/photo-1671628344495-e6bb17e0dc8b?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NXx8dHJhaW50cmFja3N8ZW58MHx8MHx8&auto=format&fit=crop&w=500&q=60-->

<!--? The website I'm basing this off of-->
<!--https://www.nytimes.com/interactive/2022/05/20/world/americas/enslaved-haiti-debt-timeline.html?unlocked_article_code=gbBkXR8Dvzax6Aa01PxdxbCTQq-VamFCGi05ArKVOONA4iTnd1dRu2B5Hcjdh0tG0OtN24QFYtC5VO2uqqqO3uaCqMpfUEQu08xCCrZ3vGqHJlJulDN2BAnwjRTzSw4-zYq5r0oS0uuFplQiOt12oMgbAun5EqbeR0THpQTGs7oPDA-OyayrutjQJKbTcpO2hfn2oV_SaTiM_TK02B8r6slCE0pkLbscRjoc50ru6pnT7ijxx8Tm2qWifCAcq5WGyOOPd3A2JUvYwuVSCb1ne62TKwtj5JNigHdsaqW4_gy5CKE44-NBTvWoe5tk3W_S9PpRcU5eBxKC0qnrguleu4zdF0yUvW3_V0y56Sv-ElsAs8piSVRIJlUQLTGp&xlid=url-share-->


<div class="bg-cover" style="background-image: url({src}); height: 880px">
	<div>
		<div class="h-80"/>
		<PageHeader header="Effect of war on genocide" subheader=" September 1, 1939 – September 2, 1945" subtext=" Gabriel Tower"/>
		<Box width=100 height=100 imagePath="https://images.unsplash.com/photo-1600267188229-1dd3dd776737?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8N3x8d29ybGQlMjB3YXIlMjAyfGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60"/>
	</div>
	<Buffer width=100 height=100/>
	<Buffer width=100 height=100/>
	<YearBreak year="War starts"/>
	<Box width=100 height=600>
		<Paragraph text="1933 Adolf Hitler came to power. During the years between 1933 - 1939, the Nazi party worked on laying the groundwork for the persecution of Jews, Homosexuals, Roma, and many other groups."/>
		<Paragraph text="These laws allowed/promoted the boycott of Jewish businesses, Evian conference, Kristallnacht, and forced emigration."/>
		<div class="w-24 h-1 bg-gray-500 mt-4"/>
		<Paragraph text=" On September 1, 1939, Hitler invaded Poland from the west; two days later, France and Britain declared war on Germany, beginning World War II."/>
		<Paragraph text="The war did not stop the persecution. It made it worse."/>
	</Box>
	<YearBreak year=1939/>
	<width width=100 height=600>
		<Header header=" Germany annexes Czechoslovakia"/>
		<ImageBox src="https://encyclopedia.ushmm.org/images/large/11282013-a4f5-4f6e-8462-32296069c3cd.jpg" width=80 height=100>
			<div class="w-24 h-1 bg-gray-500 mt-4"/>
			<p class="text-2xl">In 1933 Germany demanded that ethnic Germans in Czechoslovakia be "returned" to Germany. This also included the 
				land that they lived on. The Czechs refused and in 1938 under the direction of Hitler Germany invaded. The Germans annexed the Sudetenland. The Munich Pact was signed in 1938. 
				The pact allowed Germany to annex the Sudetenland in exchange for promised peace from Hitler.
			</p>
		</ImageBox>
		<Header header=" ST. Louis sails"/>
		<ImageBox src="data:image/jpeg;base64,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" width=10 height=30/>
		<div class="w-24 h-1 bg-gray-500 mt-4"/>
		<p class="text-2xl">In May 1939, ~900 Jews fled Germany aboard a curise liner. The ship in question was called the SS St. Louis.
			The ship was turned away from Cuba, Canada, and the United States. The ship was forced to return to Europe. 
			Many of the passengers were sent to concentration camps. "We didn't really know where we were heading, or how we would cope when we got there." - Gisela Feldman.
			With the fear of death and persecution back in mainland Europe, many were looking for a safe haven. Most of the passager would never see close family ever again.
		</p>
		<div class="w-24 h-1"/>
	</width>
	<YearBreak year=1940/>
	<Box width=100 height=600>
		<Header header=" Germany invades Poland"/>
		<div class="w-24 h-1 bg-gray-500 mt-4"/>
			<p class="text-2xl">September-October 1939, German forces implemented the infamous BiltizKreig (lightning war) and invaded Poland. The invasion was a success and the Germans quickly overran Poland. The Polish army was quickly defeated and the Polish government fled.
				Poland did have a noticeable resistance during and after the invasion. The Polish resistance was able to slow down the German advance. Note: Germany also invaded Norway and Denmark shortly after.</p>
		<br>
		<Header header="First prisoners arrive at Auschwitz"/>
		<ImageBox src="https://tinyurl.com/yp82zfjw" width=40 height=40/>
		<div class="w-24 h-1 bg-gray-500 mt-4"/>
			<p class="text-2xl">Near the Polish town Oświęcim, Nazi SS units established and large concentration camp. This camp was called Auschwitz.</p>
			<p class="text-2xl">The first prisoners were mostly Christain and Jewish men for Germany and Poland. Mostly for political reasons.</p>
			<br>
			<h1 class="text-4xl">People moved through Auschwitz from 1942 - 1944</h1>
			<br>
			<p class="text-2xl">
				Hungary: 426,000
				Poland: 300,000
				France: 69,000
				Netherlands: 60,000
				Greece: 55,000
				Bohemia and Moravia: 46,000
				Slovakia: 27,000
				Belgium: 25,000
				Yugoslavia: 10,000
				Italy: 7,500
				Norway: 690
				Other (including concentration camps): 34,000
			</p>
	</Box>
	<YearBreak year=1941/>
	<Box width=100 height=600>
		<Header header=" Mass Murder begins at Chelmno"/>
		<ImageBox src="https://tinyurl.com/2bfetkhc" width=40 height=40/>
		<div class="w-24 h-1 bg-gray-500 mt-4"/>
		<p class="text-2xl">In Poland the Nazi SS opened Chelmno killing center. Jews, Poles, POWS, and Roma were all killed. Chelmno was the first stationary facility to use gas. It was also the first camp to conduction mass murder of Jews.
			At the end of the war the Nazis attempted to burn down the camp to earse all record of it. Only two Jewish survior were found after the war.
		</p>
		<br>
		<p class="text-2xl">172,000 people were killed.</p>
	<Header header=" Germany invades Yugoslavia, Greece, and the Soviet Union"/>
		<ImageBox src="https://tinyurl.com/yfa5trps" width=40 height=40/>
		<div class="w-24 h-1 bg-gray-500 mt-4"/>
			<p class="text-2xl">Yugoslavia was aligned with the Axis but refused to allow the flow of German troops through Yugoslavia.</p>
			<p class="text-2xl">So the Germans invaded Yugoslavia on April 6, 1941.</p>
			<br>
			<p class="text-2xl">In April German, Italy, Bulgarian and Hungarian units took over Greece with relative ease. Greek resistance would continue until June of that year.</p>
	</Box>
	<YearBreak year=1942/>
	<Box width=100 height=600>
		<Header header=" Wannsee Conference"/>
		<ImageBox src="https://encyclopedia.ushmm.org/images/large/ca3ed0a2-209b-43ca-868b-4d47dcc41dbb.jpg" width=40 height=40/>
		<div class="w-24 h-1 bg-gray-500 mt-4"/>
			<p class="text-2xl">The Wannsee conference (held in Wannsee Villa in a Berlin suburb) was a meeting of Nazi party officials. The purpose of the meeting was to discuss the logistics of the "Final Solution"</p>
			<p class="text-2xl">The "Final Solution" was a euphemixl for the mass murder of European Jews. There was no question whether or not to go through with the plan, the "Final Solution" was already planned.</p>
			<p class="text-2xl">The plan didn't just include German occupied territory it extended to United Kingdom, Switzerland, Ireland, Sweden, etc... </p>
		<Header header=" Operation Reinhard"/>
		<ImageBox src="https://tinyurl.com/2rrkj5un" width=40 height=40>
		</ImageBox>
		<div class="w-24 h-1 bg-gray-500 mt-4"/>
		<p class="text-2xl">The code name for a plan to kill approximately two million Jews. Reinhard has been in the works since 1942, only 1.5 million Jews were killed during the operation.</p>
		<p class="text-2xl">Operation Reinhard had a connection with Operation T4 (Euthanaisa Program). Most of the personal in the Reinhard program came for T4, thus they had intimate knowledge gas.</p>
	</Box>
	<YearBreak year=1943/>
	<Box width=100 height=600>
		<Header header="First transport of Sinit/Roma to Auschwitz"/>
		<ImageBox src="https://tinyurl.com/3tetenur" width=100 height=100>
			<div class="w-24 h-1 bg-gray-500 mt-4"/>
			<p class="text-2xl">In 1943 the first groups of Sinit/Roma started arriving at BIIe sector.</p>
			<p class="text-2xl">Upon arriving they were not sujected to selection and families reminded together. The BIIe section was still underconstruction at the time and do to overcrowding lead to unhygenic conditions.</p>
		</ImageBox>
		<Header header=" German defeat at Stalingrad"/>
		<ImageBox src="https://tinyurl.com/58u8m7ms" width=100 height=100>
			<div class="w-24 h-1 bg-gray-500 mt-4"/>
			<p class="text-2xl">The German defeat at Stalingrad was a major turning point in the war. The Germans were forced to retreat and the Soviets were able to take back the city.<p>
			<br>
			<p class="text-2xl">Battle lasted seven months the goal was to capture the Soviet city Stalingrad (now called Volgograd). Stalingrad was the location of much of the Soviet military infrastructure.</p>
		</ImageBox>
	</Box>
	<YearBreak year=1944/>
	<Box width=100 height=600>
		<div class="w-24 h-1 mt-4"/>
		<Header header=" FDR creates war refugee board"/>
		<div class="w-24 h-1 bg-gray-500 mt-4"/>
		<p class="text-2xl">After pressure from Congress then Roosevelt created an agency whose sole job was to help Jews directly affected by the Holocaust. This simplified the support process, allowing the US to better help those affected.</p>
		<div class="w-24 h-1 mt-4"/>
		<Header header=" War ending"/>
		<div class="w-24 h-1 bg-gray-500 mt-4"/>
		<p class="text-2xl">With the surrender of Italy, D-Day, and the liberation of Auschwitz and Buchenwald by the Soviets and the US respectively. Leading to the downfall of the Nazi regime.</p>
	</Box>
	<YearBreak year=1945/>
	<Box width=100 height=200 header=" War is over">
		<p class="text-2xl">The war in Europe ended on May 8th, 1945. The war in the Pacific ended on August 15th, 1945.</p>
	</Box>
	<PageEnder/>
</div>
