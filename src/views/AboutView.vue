<template>
	<v-content>
		<!-- Intro -->
		<section id="our-vision">
			<v-container
				fluid
				class="pa-6"
				style="
					background-image: linear-gradient(to bottom left, #dbfcff, #fddcc356);
				"
				:style="{ height: 'calc(100vh - ' + $vuetify.application.top + 'px)' }"
			>
				<!-- <v-responsive
				class="pa-10"
				style="
					background-image: linear-gradient(to bottom left, #dbfcff, #fddcc356);
				"
				:max-height="{
					height: 'calc(100vh - ' + $vuetify.application.top + 'px)',
				}"
				min-width="100vw"
			> -->
				<v-layout fill-height>
					<v-flex align-self-center class="d-flex justify-center">
						<v-img
							:style="{
								height: 'calc(100vh - ' + $vuetify.application.top + 'px)',
							}"
							class="rounded"
							min-width="260"
							width="25vw"
							max-width="500"
							transition="slide-x-transition"
							:src="require('../assets/rocky-beach.jpg')"
							gradient="to bottom, rgba(0,0,0,0.2), rgba(50,0,50,.3)"
						></v-img>
					</v-flex>
					<v-flex
						align-self-center
						class="d-flex justify-center"
						style="margin-left: -55%"
					>
						<v-card
							outlined
							class="rounded-tl-xl rounded-br-xl overflow-auto"
							width="100%"
							elevation="24"
							min-width="270"
							max-width="800"
							:max-height="'calc(100vh - ' + $vuetify.application.top + 'px)'"
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
								class="text-body-2 text-sm-body-1 text-lg-h6 font-weight-light pa-5 text-justify"
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
			<!-- </v-responsive> -->
		</section>

		<!-- Sdgs -->
		<section id="sdgs">
			<v-container class="mt-10" fluid style="min-height: 60vh">
				<v-row align-content="center" justify="center">
					<v-col cols="12">
						<v-flex>
							<p class="text-h5 font-weight-bold text-center text-md-h4">
								“Plastic pollution free world is not a choice but a commitment
								to life – <br />
								a commitment to the next generation.”
							</p>
						</v-flex>
					</v-col>
				</v-row>
				<v-row justify="center">
					<v-col cols="12" style="max-width: 80vw">
						<p class="text-body-2 text-md-body-1 font-weight-bold text-left">
							We work to increase youth participation on pressing health issues.
							Our ambition is to create empowering spaces for cooperative
							dialogue and action where youth showcase talent and launch
							initiatives. Lorem ipsum dolor sit amet consectetur adipisicing
							elit. Consequuntur itaque iste adipisci labore, nemo expedita.
						</p>
					</v-col>
				</v-row>
				<v-row justify="center" class="pt-1">
					<v-col cols="2">
						<v-img
							min-width="50"
							max-width="150"
							transition="slide-x-transition"
							:src="require('../assets/sdg-14.png')"
						></v-img>
					</v-col>

					<v-col cols="2">
						<v-img
							min-width="50"
							max-width="150"
							transition="slide-x-transition"
							:src="require('../assets/sdg-15.png')"
						></v-img>
					</v-col>
					<v-col cols="2">
						<v-img
							min-width="50"
							max-width="150"
							transition="slide-x-transition"
							:src="require('../assets/sdg-12.png')"
						></v-img>
					</v-col>
					<v-col cols="2">
						<v-img
							min-width="50"
							max-width="150"
							transition="slide-x-transition"
							:src="require('../assets/sdg-13.jpg')"
						></v-img>
					</v-col>
					<v-col cols="2">
						<v-img
							min-width="50"
							max-width="150"
							transition="slide-x-transition"
							:src="require('../assets/sdg-10.png')"
						></v-img>
					</v-col>
				</v-row>
			</v-container>
		</section>
		<div class="py-10 hidden-sm-and-up"></div>

		<!-- Five principles intro -->
		<section id="five-principles-intro">
			<v-container fluid style="padding: 0" class="hidden-xs-and-down">
				<v-divider style="background: grey"></v-divider>
				<!-- <span class="wavey__line"></span> -->

				<v-layout fill-height>
					<v-row no-gutters>
						<v-col cols="4">
							<v-container
								fill-height
								fluid
								style="
									color: white;
									background-image: linear-gradient(to top, blue, #3fa9f5);
								"
								class="rounded-r-xl"
							>
								<v-row>
									<v-col align="left">
										<v-lazy>
											<div
												class="text-subtitle-1 text-sm-h5 text-md-h4 text-uppercase font-weight-bold"
											>
												5 <br />
												Issues
											</div>
										</v-lazy>
									</v-col>
								</v-row>
								<v-row>
									<v-col>
										<v-lazy>
											<div
												class="text-subtitle-1 text-sm-h5 text-md-h4 text-uppercase font-weight-bold"
											>
												5 <br />
												Principles
											</div>
										</v-lazy>
									</v-col>
								</v-row>
								<v-row>
									<v-col>
										<v-lazy>
											<div
												class="text-subtitle-1 text-sm-h5 text-md-h4 text-uppercase font-weight-bold"
											>
												5 <br />
												Outcomes
											</div>
										</v-lazy>
									</v-col>
								</v-row>
							</v-container>
						</v-col>
						<div style="height: 75vh"></div>
						<v-col>
							<v-container
								class="d-flex justify-center ma-2"
								fill-height
								style="background: inherit"
							>
								<v-row no-gutters>
									<v-col class="d-flex justify-center align-center">
										<v-card
											class="rounded text-center overflow-auto pa-10"
											width="100%"
											flat
											style="background: whitesmoke; max-height: 100%"
										>
											<v-card-title
												class="text-h4 text-sm-h3 font-weight-bold mb-3 text-uppercase text-left"
												>Our <br />
												Belief
											</v-card-title>
											<v-card-subtitle>
												<v-responsive width="56">
													<v-divider class="mb-1"></v-divider>
													<v-divider></v-divider>
												</v-responsive>
											</v-card-subtitle>
											<p
												class="text-body-2 text-sm-body-1 text-lg-h6 font-weight-light pa-2 text-justify"
											>
												Follow our <strong>5x5x5 framework</strong> to
												understand how we generate impact, beginning with
												identifying the key problems, then applying key pillar
												principles, and finally creating impactful outcomes.
												<br />
												Lorem ipsum dolor sit amet consectetur adipisicing elit.
												Debitis reprehenderit ut optio iusto distinctio ipsa
												labore architecto temporibus dolor mollitia dicta saepe
												suscipit
											</p>
										</v-card>
									</v-col>
								</v-row>
								<v-row class="d-flex justify-center">
									<v-col class="d-flex align-center justify-center">
										<v-timeline
											style="max-height: fit-content"
											class="text-md-h6"
											dense
										>
											<v-timeline-item icon="mdi-alert" fill-dot color="pink">
												Identify the <br />
												<strong> Key Issue</strong>
											</v-timeline-item>
											<v-timeline-item
												icon="mdi-head-lightbulb-outline"
												fill-dot
												color="cyan"
											>
												Creating a solution via applying a <br />
												<strong>Key Principle</strong>
											</v-timeline-item>
											<v-timeline-item icon="mdi-star" fill-dot>
												Generate an <strong>Impactful Outcome</strong>
											</v-timeline-item>
										</v-timeline>
									</v-col>
								</v-row>
							</v-container>
						</v-col>
					</v-row>
				</v-layout>
				<!-- <v-divider style="background: grey"></v-divider> -->
			</v-container>
		</section>

		<section id="five-principles">
			<div style="min-height: 100vh">
				<v-responsive>
					<v-img :src="require('../assets/waves-background.png')"></v-img>
				</v-responsive>

				<v-container
					class="text-center text-h3 text-sm-h2 font-weight-bold mb-3 text-uppercase"
					style="margin-top: -8%"
				>
					Five Framework
					<div class="py-1"></div>
					<v-responsive width="100" class="mx-auto">
						<v-divider class="mb-1" style="background: whitesmoke"></v-divider>
						<v-divider style="background: white"></v-divider>
					</v-responsive>
				</v-container>

				<div class="py-3"></div>
				<div>
					<SlidesPage></SlidesPage>
				</div>
			</div>
		</section>
		<div class="py-8"></div>
	</v-content>
</template>

<script>
import SlidesPage from "../components/SlidesPage.vue";
export default {
	components: { SlidesPage },
	data() {
		return {
			window: 0,
		};
	},
};
</script>
