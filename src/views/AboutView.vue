<template>
	<v-content>
		<!-- Intro -->
		<section id="our-vision">
			<v-container
				fluid
				class="pa-10"
				style="
					background-image: linear-gradient(to bottom left, #dbfcff, #fddcc356);
				"
				:style="{ height: 'calc(100vh - ' + $vuetify.application.top + 'px)' }"
			>
				<v-layout fill-height>
					<v-flex align-self-center class="d-flex justify-center">
						<v-img
							:style="{
								height: 'calc(100vh - ' + $vuetify.application.top + 'px)',
							}"
							width="20vw"
							min-width="300"
							max-width="500"
							transition="slide-x-transition"
							:src="require('../assets/rocky-beach.jpg')"
							gradient="to bottom, rgba(0,0,0,0.2), rgba(50,0,50,.3)"
						></v-img>
					</v-flex>
					<v-flex
						align-self-center
						class="d-flex justify-center"
						style="margin-left: -45%"
					>
						<v-card
							outlined
							max-height="80vh"
							class="rounded-tl-xl rounded-br-xl overflow-auto"
							width="90%"
							max-width="800"
							color="#274156"
							dark
						>
							<v-card-title
								class="text-h4 text-sm-h3 font-weight-bold mb-3 text-uppercase"
								>Our Vision</v-card-title
							>
							<v-card-subtitle>
								<v-responsive width="56">
									<v-divider
										class="mb-1"
										style="background: whitesmoke"
									></v-divider>
									<v-divider style="background: white"></v-divider>
								</v-responsive>
							</v-card-subtitle>
							<p
								class="text-body-1 text-sm-h6 font-weight-light pa-2 text-justify"
							>
								We envision a better world where technology helps us to bridge
								the gap between our desire for a healthy planet and achievable +
								actionable solutions. We hope that through education and
								demonstrating the power of current technology, we can empower
								communities to be fearless at solving the ocean pollution
								problem themselves.
							</p>
							<v-btn
								class="ma-3 align-self-center"
								fab
								outlined
								@click="$vuetify.goTo('#sdgs')"
							>
								<v-icon>mdi-chevron-double-down</v-icon>
							</v-btn>
						</v-card>
					</v-flex>
				</v-layout>
			</v-container>
		</section>

		<!-- Sdgs -->
		<section id="sdgs">
			<v-container class="mt-10" fluid style="min-height: 60vh">
				<v-row align-content="center" justify="center">
					<v-col cols="8">
						<v-flex>
							<p class="text-h5 font-weight-bold text-center text-md-h4">
								“Plastic pollution free world is not a choice but a commitment
								to life – a commitment to the next generation.”
							</p>
						</v-flex>
					</v-col>
				</v-row>
				<v-row justify="center">
					<v-col cols="10" style="max-width: 70vw">
						<p class="text-body-2 text-md-body-1 font-weight-bold text-left">
							We work to increase youth participation on pressing health issues.
							Our ambition is to create empowering spaces for cooperative
							dialogue and action where youth showcase talent and launch
							initiatives.
						</p>
					</v-col>
				</v-row>
				<v-row justify="center" class="pt-1">
					<v-col cols="2">
						<v-img
							max-width="150"
							transition="slide-x-transition"
							:src="require('../assets/sdg-14.png')"
						></v-img>
					</v-col>

					<v-col cols="2">
						<v-img
							max-width="150"
							transition="slide-x-transition"
							:src="require('../assets/sdg-15.png')"
						></v-img>
					</v-col>
					<v-col cols="2">
						<v-img
							max-width="150"
							transition="slide-x-transition"
							:src="require('../assets/sdg-12.png')"
						></v-img>
					</v-col>
					<v-col cols="2">
						<v-img
							max-width="150"
							transition="slide-x-transition"
							:src="require('../assets/sdg-13.jpg')"
						></v-img>
					</v-col>
					<v-col cols="2">
						<v-img
							max-width="150"
							transition="slide-x-transition"
							:src="require('../assets/sdg-10.png')"
						></v-img>
					</v-col>
				</v-row>
			</v-container>
		</section>
		<div class="py-10"></div>
		<!-- Five principles intro -->
		<section id="five-principles-intro" style="height: 80vh">
			<v-container fluid style="height: 100%; padding: 0">
				<v-divider style="background: #3fa9f5"></v-divider>
				<v-layout fill-height>
					<v-row>
						<v-col cols="4">
							<v-container
								fill-height
								style="
									color: white;
									background-image: linear-gradient(-45deg, blue, #3fa9f5);
								"
							>
								<v-row class="pa-2">
									<v-col align="left">
										<v-lazy>
											<div
												class="text-h6 text-md-h5 text-uppercase font-weight-bold"
											>
												5 Issues
											</div>
										</v-lazy>
									</v-col>
								</v-row>
								<v-row class="pa-2">
									<v-col align="center">
										<v-lazy>
											<div
												class="text-h6 text-md-h5 text-uppercase font-weight-bold"
											>
												5 Principles
											</div>
										</v-lazy>
									</v-col>
								</v-row>
								<v-row class="pa-2 py-1">
									<v-col align="right">
										<v-lazy>
											<div
												class="text-h6 text-md-h5 text-uppercase font-weight-bold"
											>
												5 Outcomes
											</div>
										</v-lazy>
									</v-col>
								</v-row>
							</v-container>
						</v-col>

						<v-col cols="8">
							<v-container
								class="d-flex justify-center"
								fill-height
								style="background: inherit"
							>
								<v-row>
									<v-lazy>
										<v-card
											class="rounded text-center overflow-auto"
											width="95%"
											elevation="10"
											style="background: whitesmoke; max-height: 70vh"
										>
											<v-card-title
												class="text-h4 text-sm-h3 font-weight-bold mb-3 text-uppercase"
												>Our Mission</v-card-title
											>
											<v-card-subtitle>
												<v-responsive width="56">
													<v-divider class="mb-1"></v-divider>
													<v-divider></v-divider>
												</v-responsive>
											</v-card-subtitle>
											<p
												class="text-body-1 text-sm-h6 font-weight-light pa-2 text-justify"
											>
												Follow our <strong>5x5x5 framework</strong> to
												understand how we generate impact, beginning with
												identifying the key problems, then applying key pillar
												principles, and finally creating impactful outcomes.
												<br />
												Lorem ipsum dolor sit amet consectetur adipisicing elit.
												Debitis reprehenderit ut optio iusto distinctio ipsa
												labore architecto temporibus dolor mollitia dicta saepe
												suscipit laudantium accusantium, exercitationem odit?
												Quia voluptates amet non. Corporis officiis et assumenda
												laboriosam doloribus? Repellendus, corrupti labore.
											</p>
										</v-card>
									</v-lazy>
								</v-row>
								<v-row class="d-flex justify-center">
									<div>
										<v-timeline>
											<v-timeline-item>
												Identify the <strong> Key Issue</strong>
											</v-timeline-item>
											<v-timeline-item class="text-right">
												Creating a solution via applying a <br />
												<strong>Core Principle</strong>
											</v-timeline-item>
											<v-timeline-item>
												Generate an <strong>Impactful Outcome</strong>
											</v-timeline-item>
										</v-timeline>
									</div>
								</v-row>
							</v-container>
						</v-col>
					</v-row>
				</v-layout>
				<v-divider style="background: #3fa9f5"></v-divider>
			</v-container>
		</section>

		<section id="five-principles">
			<v-container fluid style="min-height: 80vh">
				<!-- <div class="pa-2">
					<v-stepper non-linear vertical>
						<v-stepper-step complete editable step="1">
							Identify the <strong>Issue</strong>
						</v-stepper-step>
						<v-stepper-content class="mb-1" step="1">
							<v-card
								color="grey lighten-1"
								class="mb-12"
								height="200px"
							></v-card>
							<v-btn color="primary"> Continue </v-btn>
							<v-btn text> Cancel </v-btn>
						</v-stepper-content>

						<v-stepper-step editable step="2">
							Creating a solution via applying a <strong>Principle</strong>
						</v-stepper-step>

						<v-stepper-content class="mb-1" step="2">
							<v-card outlined class="mb-12" height="100px">
								<v-card-title
									>Lorem ipsum dolor sit amet consectetur adipisicing elit.
									Ipsam, cumque.</v-card-title
								>
							</v-card>
						</v-stepper-content>

						<v-stepper-step active editable step="3">
							Generate an Impactful <strong>Outcome</strong>
						</v-stepper-step>

						<v-stepper-content step="3">
							<v-card class="mb-12" height="100px">
								<v-card-title
									>Lorem ipsum dolor sit amet consectetur adipisicing elit.
									Ipsam, cumque.</v-card-title
								>
							</v-card>
						</v-stepper-content>
					</v-stepper>
				</div> -->
				<v-card width="50vw" class="pa-7" outlined>
					<v-row align="center">
						<v-item-group
							v-model="window"
							class="shrink mr-6"
							mandatory
							tag="v-flex"
						>
							<v-item v-for="s in array" :key="s" v-slot="{ active, toggle }">
								<div>
									<v-btn :input-value="active" icon @click="toggle">
										<v-icon>mdi-record</v-icon>
									</v-btn>
								</div>
							</v-item>
						</v-item-group>
						<v-col>
							<v-window v-model="window" vertical class="elevation-2">
								<v-window-item v-for="s in array" :key="s">
									<v-card flat>
										<v-card-text>
											<p>{{ s }}</p>
										</v-card-text>
									</v-card>
								</v-window-item>
							</v-window>
						</v-col>
					</v-row>
				</v-card>
			</v-container>
		</section>
	</v-content>
</template>
<script>
export default {
	data() {
		return {
			window: 0,
			array: [
				"Human Psychology",
				"Encourage Learning",
				"Real-time and engaging approach to the ocean pollution education",
			],
			fiveFramework: [
				{
					issue: "Human Psychology",
					principle: "Encourage Learning",
					outcome:
						"Real-time and engaging approach to the ocean pollution education",
				},
				{
					issue: "Personal Connection",
					principle: "Improve Knowledge Translation",
					outcome: "Effective communication that incentivises action",
				},
				{
					issue: "Feasibility of Problem Solving",
					principle: "Foster Changes in Attitudes",
					outcome: "Developing a personal connection to the problem",
				},
				{
					issue: "Knowledge Translation",
					principle: "Maintain Transparency",
					outcome:
						"Provide transparency and combat mistrust about its dangers ",
				},
				{
					issue: "Scepticism",
					principle: "Promote Youth Engagement",
					outcome:
						"Youth engagement and advocacy development to inspire collective intergenerational action",
				},
			],
		};
	},
};
</script>
