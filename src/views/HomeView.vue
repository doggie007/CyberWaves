<template>
	<v-content>
		<section id="hero">
			<!-- <v-expand-transition> -->
			<v-slide-y-transition>
				<v-row no-gutters>
					<v-img
						:height="'calc(100vh - ' + $vuetify.application.top + 'px)'"
						:src="require('../assets/ocean-cover.jpg')"
						gradient="to top right, rgba(0,0,0,0.35), rgba(0,0,0,.7)"
						transition="slide-x-transition"
						dark
					>
						<v-theme-provider dark>
							<v-container fill-height>
								<v-row
									align="center"
									class="white--text mx-auto"
									justify="center"
								>
									<v-col class="white--text text-start" cols="12" tag="h1">
										<span
											class="font-weight-light text-h4 text-sm-h3 text-md-h2"
										>
											WELCOME TO
										</span>

										<br />

										<span
											class="font-weight-black text-h3 text-sm-h2 text-md-h1"
										>
											CYBERWAVES
										</span>
										<br />
										<div class="py-4"></div>
										<span class="font-weight-light text-h6 text-sm-h5">
											Empowering a wave of technological change to save our
											oceans.</span
										>
									</v-col>
									<v-spacer></v-spacer>
									<v-btn
										class="align-self-end mt-12"
										fab
										outlined
										@click="$vuetify.goTo('#about')"
									>
										<v-icon>mdi-chevron-double-down</v-icon>
									</v-btn>
								</v-row>
							</v-container>
						</v-theme-provider>
					</v-img>
				</v-row>
			</v-slide-y-transition>
			<!-- </v-expand-transition> -->
		</section>

		<!-- About Section -->
		<section id="about">
			<div class="py-12"></div>

			<v-container class="text-center">
				<h2 class="display-2 font-weight-bold mb-3 pa-1">OUR MISSION</h2>

				<v-responsive class="mx-auto mb-8" width="56">
					<v-divider class="mb-1"></v-divider>
					<v-divider></v-divider>
				</v-responsive>

				<v-responsive
					class="pa-2 mx-auto title font-weight-light mb-8 text-justify"
					max-width="720"
				>
					We strive to raise awareness of the gravity of the
					<strong>ocean pollution problem</strong> through utilisation of
					technological advances such as
					<strong>AI and satellite imaging</strong>, endeavouring to combat
					public disengagement and encourage collaborative action. <br />
					Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quasi
					explicabo, atque libero veniam repellat dignissimos quod rem eaque
					error cupiditate.
				</v-responsive>

				<v-row class="mx-auto" no-gutters>
					<v-col>
						<v-avatar class="elevation-12 mb-12" size="128">
							<v-img src=""></v-img>
						</v-avatar>
						<div class="text-h6">Name Here</div>
					</v-col>
					<v-col>
						<v-avatar class="elevation-12 mb-12" size="128">
							<v-img src=""></v-img>
						</v-avatar>
						<div class="text-h6">Name Here</div>
					</v-col>
					<v-col>
						<v-avatar class="elevation-12 mb-12" size="128">
							<v-img src=""></v-img>
						</v-avatar>
						<div class="text-h6">Name Here</div>
					</v-col>
				</v-row>

				<div class="py-5"></div>

				<v-btn color="grey" outlined large link to="/about">
					<span class="grey--text text--darken-1 font-weight-bold">
						Learn More
					</span>
				</v-btn>
				<div class="py-10"></div>
			</v-container>
		</section>

		<!-- <section id="features" class="grey lighten-3">
				<div class="py-12"></div>

				<v-container class="text-center">
					<h2 class="display-2 font-weight-bold mb-3">VUETIFY FEATURES</h2>

					<v-responsive class="mx-auto mb-12" width="56">
						<v-divider class="mb-1"></v-divider>

						<v-divider></v-divider>
					</v-responsive>

					<v-row>
						<v-col
							v-for="({ icon, title, text }, i) in features"
							:key="i"
							cols="12"
							md="4"
						>
							<v-card class="py-12 px-4" color="grey lighten-5" flat>
								<v-theme-provider dark>
									<div>
										<v-avatar color="primary" size="88">
											<v-icon large v-text="icon"></v-icon>
										</v-avatar>
									</div>
								</v-theme-provider>

								<v-card-title
									class="justify-center font-weight-black text-uppercase"
									v-text="title"
								></v-card-title>

								<v-card-text class="subtitle-1" v-text="text"> </v-card-text>
							</v-card>
						</v-col>
					</v-row>
				</v-container>

				<div class="py-12"></div>
			</section> -->

		<!-- Impact Section -->
		<section id="impact">
			<v-parallax
				:height="$vuetify.breakpoint.smAndDown ? 700 : 500"
				:src="require('../assets/dimmed-forest.jpg')"
			>
				<v-container fill-height justify-center>
					<v-row></v-row>
					<v-row>
						<v-col
							v-for="[value, title] of stats"
							:key="title"
							cols="12"
							md="4"
						>
							<div class="text-center">
								<div
									class="display-3 font-weight-black mb-4"
									v-text="value"
								></div>

								<div
									class="title font-weight-regular text-uppercase"
									v-text="title"
								></div>
							</div>
						</v-col>
					</v-row>
					<div>
						<v-btn class="fb-btn" elevation="24" large rounded dark>
							Learn more about Our Impact
							<v-icon>mdi-chevron-right</v-icon>
						</v-btn>
					</div>
				</v-container>
			</v-parallax>
		</section>

		<!-- Technology display -->
		<section id="blog">
			<div class="py-12"></div>

			<v-container>
				<h2
					class="text-h4 text-sm-h3 font-weight-bold mb-3 text-center text-uppercase"
				>
					Latest Open-Source Technology
				</h2>

				<v-responsive class="mx-auto mb-12 text-left" width="56">
					<v-divider class="mb-1"></v-divider>
					<v-divider></v-divider>
				</v-responsive>

				<v-row>
					<v-col
						v-for="({ src, text, title }, i) in articles"
						:key="i"
						cols="12"
						md="4"
					>
						<v-img
							:src="src"
							class="mb-4"
							height="275"
							max-width="100%"
						></v-img>

						<h3
							class="font-weight-black mb-4 text-uppercase"
							v-text="title"
						></h3>

						<div class="title font-weight-light mb-5" v-text="text"></div>

						<v-btn class="ml-0 font-weight-black" outlined>
							Continue Reading
						</v-btn>
					</v-col>
				</v-row>
			</v-container>

			<div class="py-12"></div>
		</section>
	</v-content>
</template>

<style scoped>
.fb-btn {
	border: 2px solid #000;
}
</style>

<script>
export default {
	name: "Home",
	data() {
		return {
			show: true,
			articles: [
				{
					src: "https://images.unsplash.com/photo-1423784346385-c1d4dac9893a?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1950&q=80",
					title: "Some Cool Tech",
					text: "Phasellus lorem enim, luctus ut velit eget, convallis egestas eros. Sed ornare ligula eget tortor tempor, quis porta tellus dictum.",
				},
				{
					src: "https://images.unsplash.com/photo-1475938476802-32a7e851dad1?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1950&q=80",
					title: "Some Cool Tech",
					text: "Nam ut leo ipsum. Maecenas pretium aliquam feugiat. Aenean vel tempor est, vitae tincidunt risus. Sed sodales vestibulum nibh.",
				},
				{
					src: "https://images.unsplash.com/photo-1416339442236-8ceb164046f8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1892&q=80",
					title: "Some Cool Tech",
					text: "Vestibulum in dictum velit, in rhoncus nibh. Maecenas neque libero, interdum a dignissim in, aliquet vitae lectus. Phasellus lorem enim, luctus ut velit eget.",
				},
			],
			features: [
				{
					icon: "mdi-account-group-outline",
					title: "Vibrant Community",
					text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto cupiditate sint possimus quidem atque harum excepturi nemo velit tempora! Enim inventore fuga, qui ipsum eveniet facilis obcaecati corrupti asperiores nam",
				},
				{
					icon: "mdi-update",
					title: "Frequent Updates",
					text: "Sed ut elementum justo. Suspendisse non justo enim. Vestibulum cursus mauris dui, a luctus ex blandit. Lorem ipsum dolor sit amet consectetur adipisicing elit. qui ipsum eveniet facilis obcaecati corrupti consectetur adipisicing elit.",
				},
				{
					icon: "mdi-shield-outline",
					title: "Long-term Support",
					text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto cupiditate sint possimus quidem atque harum excepturi nemo velit tempora! Enim inventore fuga, qui ipsum eveniet facilis obcaecati corrupti asperiores nam",
				},
			],
			stats: [
				["3", "Organisation partners"],
				["10k", "Users"],
				["40m", "Funding"],
			],
		};
	},
};
</script>
