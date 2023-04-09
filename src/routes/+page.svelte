<script lang="ts">
    import Header from '../lib/Header.svelte';
    import Box from '../lib/Box.svelte';
	import YearBreak from '$lib/YearBreak.svelte';
	import PageEnder from '$lib/PageEnder.svelte';
	import Buffer from '$lib/Buffer.svelte';
	import Paragraph from '$lib/Paragraph.svelte';
	import PageHeader from '../lib/PageHeader.svelte';
	import ImageBox from '../lib/ImageBox.svelte';
	import VBuffer from '../lib/VBuffer.svelte';

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
<!--https://www.nytimes.com/interactive/2022/05/20/world/americas/enslaved-haiti-debt-timeline.html?unlocked_article_code=gbBkXR8Dvzax6Aa01PxdxbCTQq-VamFCGi05ArKVOONA4iTnd1dRu2B5Hcjdh0tG0OtN24QFYtC5VO2uqqqO3uaCqMpfUEQu08xCCrZ3vGqHJlJulDN2BAnwjRTzSw4-zYq5r0oS0uuFplQiOt12oMgbAun5EqbeR0THpQTGs7oPDA-OyayrutjQJKbTcpO2hfn2oV_SaTiM_TK02B8r6slCE0pkLbscRjoc50ru6pnT7ijxx8Tm2qWifCAcq5WGyOOPd3A2JUvYwuVSCb1ne62TKwtj5JNigHdsaqW4_gy5CKE44-NBTvWoe5tk3W_S9PpRcU5eBxKC0qnrguleu4zdF0yUvW3_V0y56Sv-ElsAs8piSVRIJlUQLTGp&smid=url-share-->


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
			<p class="text-2sm">In 1933 Germany demanded that ethnic Germans in Czechoslovakia be "returned" to Germany. This also included the 
				land that they lived on. The Czechs refused and in 1938 under the direction of Hitler Germany invaded. The Germans annexed the Sudetenland. The Munich Pact was signed in 1938. 
				The pact allowed Germany to annex the Sudetenland in exchange for promised peace from Hitler.
			</p>
		</ImageBox>
		<Header header=" ST. Louis sails"/>
		<ImageBox src="https://www.facinghistory.org/sites/default/files/styles/social_image_1200x630_1x/public/2022-06/Holocaust_1939_RefugeesAboardTheStLouis_%20FH229460.jpg?h=8911ddd7&itok=lQ6lcvlf" width=10 height=10>
			<div class="w-24 h-1 bg-gray-500 mt-4"/>
			<p class="text-2sm">In May 1939, ~900 Jews fled Germany aboard a curise liner. The ship in question was called the SS St. Louis.
				The ship was turned away from Cuba, Canada, and the United States. The ship was forced to return to Europe. 
				Many of the passengers were sent to concentration camps. "We didn't really know where we were heading, or how we would cope when we got there." - Gisela Feldman.
				With the fear of death and persecution back in mainland Europe, many were looking for a safe haven. Most of the passager would never see close family ever again.
			</p>
		</ImageBox>
		<div class="w-24 h-1"/>
	</width>
	<YearBreak year=1940/>
	<Box width=100 height=600>
		<Header header=" Germany invades Poland"/>
		<ImageBox src="" width=40 height=40>
			<div class="w-24 h-1 bg-gray-500 mt-4"/>
			<p class="text-2sm">September-October 1939, German forces implemented the infamous BiltizKreig (lightning war) and invaded Poland. The invasion was a success and the Germans quickly overran Poland. The Polish army was quickly defeated and the Polish government fled.
				Poland did have a noticeable resistance during and after the invasion. The Polish resistance was able to slow down the German advance. Note: Germany also invaded Norway and Denmark shortly after.</p>
		</ImageBox>
		<Header header="First prisoners arrive at Auschwitz"/>
		<ImageBox src="https://tinyurl.com/yp82zfjw" width=40 height=40>
			<div class="w-24 h-1 bg-gray-500 mt-4"/>
			<p class="text-2sm">Near the Polish town Oświęcim, Nazi SS units established and large concentration camp. This camp was called Auschwitz.</p>
			<p class="text-2sm">The first prisoners were mostly Christain and Jewish men for Germany and Poland. Mostly for political reasons.</p>
		</ImageBox>
	</Box>
	<YearBreak year=1941/>
	<Box width=100 height=600>
		<Header header=" Mass Murder begins at Chelmno"/>
		<ImageBox src="https://tinyurl.com/2bfetkhc" width=40 height=40>
			<div class="w-24 h-1 bg-gray-500 mt-4"/>
			<p class="text-2sm">In Poland the Nazi SS opened Chelmno killing center. Jews, Poles, POWS, and Roma were all killed. Chelmno was the first stationary facility to use gas.</p>
			<br>
			<p class="text-2sm">172,000 people were killed.</p>
		</ImageBox>
		<Header header=" Germany invades Yugoslavia, Greece, and the Soviet Union"/>
		<ImageBox src="https://tinyurl.com/yfa5trps" width=40 height=40>
			<div class="w-24 h-1 bg-gray-500 mt-4"/>
			<p class="text-2sm">Yugoslavia was aligned with the Axis but refused to allow the flow of German troops through Yugoslavia.</p>
			<p class="text-2sm">So the Germans invaded Yugoslavia on April 6, 1941.</p>
			<br>
			<p class="text-2sm">In Aptil Germann, Italy, Bulgarian and Hungarian units took over Greece with relative ease. Greek resistance would continue until June of that year.</p>
		</ImageBox>
	</Box>
	<YearBreak year=1942/>
	<Box width=100 height=600>
		<Header header=" Wannsee Conference"/>
		<ImageBox src="https://encyclopedia.ushmm.org/images/large/ca3ed0a2-209b-43ca-868b-4d47dcc41dbb.jpg" width=40 height=40>
			<div class="w-24 h-1 bg-gray-500 mt-4"/>
			<p class="text-2sm">The Wannsee conference (held in Wannsee Villa in a Berlin suburb) was a meeting of Nazi party officials. The purpose of the meeting was to discuss the logistics of the "Final Solution"</p>
			<p class="text-2sm">The "Final Solution" was a euphemism for the mass murder of European Jews.</p>
		</ImageBox>
		<Header header=" Operation Reinhard"/>
		<ImageBox src="https://tinyurl.com/2rrkj5un" width=40 height=40>
		</ImageBox>
		<div class="w-24 h-1 bg-gray-500 mt-4"/>
		<p class="text-2sm">The code name for a plan to kill approximately two million Jews. Reinhard has been in the works since 1942, only 1.5 million Jews were killed during the operation.</p>
	</Box>
	<YearBreak year=1943/>
	<Box width=100 height=600>
		<Header header="First transport of Sinit/Roma to Auschwitz"/>
		<ImageBox src="https://tinyurl.com/3tetenur" width=100 height=100>
			<div class="w-24 h-1 bg-gray-500 mt-4"/>
			<p class="text-2sm">In 1943 the first groups of Sinit/Roma started arriving at Auschwitz-Birkenau. They were originally placed in family camps and kept together.</p>
		</ImageBox>
		<Header header=" German defeat at Stalingrad"/>
		<ImageBox src="https://tinyurl.com/58u8m7ms" width=100 height=100>
			<div class="w-24 h-1 bg-gray-500 mt-4"/>
			<p class="text-2sm">The German defeat at Stalingrad was a major turning point in the war. The Germans were forced to retreat and the Soviets were able to take back the city.<p>
			<br>
			<p class="text-2sm">Battle lasted seven months the goal was to capture the Soviet city Stalingrad (now called Volgograd). Stalingrad was the location of much of the Soviet military infrastructure.</p>
		</ImageBox>
	</Box>
	<YearBreak year=1944/>
	<Box width=100 height=600>
		<div class="w-24 h-1 mt-4"/>
		<Header header=" FDR creates war refugee board"/>
		<div class="w-24 h-1 bg-gray-500 mt-4"/>
		<p class="text-2sm">After pressure from Congress then Roosevelt created an agency whose sole job was to help Jews directly affected by the Holocaust. This simplified the support process, allowing the US to better help those affected.</p>
		<div class="w-24 h-1 mt-4"/>
		<Header header=" War ending"/>
		<div class="w-24 h-1 bg-gray-500 mt-4"/>
		<p class="text-2sm">With the surrender of Italy, D-Day, and the liberation of Auschwitz and Buchenwald by the Soviets and the US respectively. Leading to the downfall of the Nazi regime.</p>
	</Box>
	<YearBreak year=1945/>
	<Box width=100 height=200 header=" War is over">
		<p class="text-2sm">The war in Europe ended on May 8th, 1945. The war in the Pacific ended on August 15th, 1945.</p>
	</Box>
	<PageEnder/>
</div>
