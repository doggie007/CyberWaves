<template>
	<v-container>
		<v-row>
			<v-card tile>
				<v-window v-model="onboarding" vertical>
					<SlidesItem
						v-for="(item, i) in fiveFramework"
						:key="`card-${i}`"
						:item="item"
						:number="i"
					></SlidesItem>
				</v-window>

				<v-card-actions class="justify-space-between">
					<v-btn text @click="prev">
						<v-icon>mdi-chevron-left</v-icon>
					</v-btn>
					<v-item-group v-model="onboarding" class="text-center" mandatory>
						<v-row>
							<v-col v-for="(item, n) in fiveFramework" :key="`btn-${n}`">
								<v-item v-slot="{ active, toggle }" class="px-auto">
									<v-btn icon small :input-value="active" @click="toggle">
										<!-- <v-icon>mdi-record</v-icon> -->
										{{ n + 1 }}
									</v-btn>
								</v-item>
							</v-col>
						</v-row>
					</v-item-group>
					<v-btn text @click="next">
						<v-icon>mdi-chevron-right</v-icon>
					</v-btn>
				</v-card-actions>
			</v-card>
		</v-row>
	</v-container>
</template>

<script>
import SlidesItem from "./SlidesItem.vue";
export default {
	components: ["SlidesItem"],
	data: () => ({
		length: 5,
		onboarding: 0,
		fiveFramework: [
			{
				issue: "Human Psychology",
				issueDescription:
					"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis excepturi labore similique repellat aspernatur? Cumque corrupti quod debitis et ex illum, eum ducimus totam blanditiis eius, natus deserunt nesciunt veritatis?",
				principle: "Encourage Learning",
				principleDescription:
					"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis excepturi labore similique repellat aspernatur? Cumque corrupti quod debitis et ex illum, eum ducimus totam blanditiis eius, natus deserunt nesciunt veritatis?",
				outcome:
					"Real-time and engaging approach to the ocean pollution education",
				outcomeDescription:
					"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis excepturi labore similique repellat aspernatur? Cumque corrupti quod debitis et ex illum, eum ducimus totam blanditiis eius, natus deserunt nesciunt veritatis?",
			},
			{
				issue: "Personal Connection",
				issueDescription:
					"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis excepturi labore similique repellat aspernatur? Cumque corrupti quod debitis et ex illum, eum ducimus totam blanditiis eius, natus deserunt nesciunt veritatis?",
				principle: "Improve Knowledge Translation",
				principleDescription:
					"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis excepturi labore similique repellat aspernatur? Cumque corrupti quod debitis et ex illum, eum ducimus totam blanditiis eius, natus deserunt nesciunt veritatis?",
				outcome: "Effective communication that incentivises action",
				outcomeDescription:
					"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis excepturi labore similique repellat aspernatur? Cumque corrupti quod debitis et ex illum, eum ducimus totam blanditiis eius, natus deserunt nesciunt veritatis?",
			},
			{
				issue: "Feasibility of Problem Solving",
				issueDescription:
					"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis excepturi labore similique repellat aspernatur? Cumque corrupti quod debitis et ex illum, eum ducimus totam blanditiis eius, natus deserunt nesciunt veritatis?",
				principle: "Foster Changes in Attitudes",
				principleDescription:
					"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis excepturi labore similique repellat aspernatur? Cumque corrupti quod debitis et ex illum, eum ducimus totam blanditiis eius, natus deserunt nesciunt veritatis?",
				outcome: "Developing a personal connection to the problem",
				outcomeDescription:
					"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis excepturi labore similique repellat aspernatur? Cumque corrupti quod debitis et ex illum, eum ducimus totam blanditiis eius, natus deserunt nesciunt veritatis?",
			},
			{
				issue: "Knowledge Translation",
				issueDescription:
					"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis excepturi labore similique repellat aspernatur? Cumque corrupti quod debitis et ex illum, eum ducimus totam blanditiis eius, natus deserunt nesciunt veritatis?",
				principle: "Maintain Transparency",
				principleDescription:
					"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis excepturi labore similique repellat aspernatur? Cumque corrupti quod debitis et ex illum, eum ducimus totam blanditiis eius, natus deserunt nesciunt veritatis?",
				outcome: "Provide transparency and combat mistrust about its dangers ",
				outcomeDescription:
					"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis excepturi labore similique repellat aspernatur? Cumque corrupti quod debitis et ex illum, eum ducimus totam blanditiis eius, natus deserunt nesciunt veritatis?",
			},
			{
				issue: "Scepticism",
				issueDescription:
					"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis excepturi labore similique repellat aspernatur? Cumque corrupti quod debitis et ex illum, eum ducimus totam blanditiis eius, natus deserunt nesciunt veritatis?",
				principle: "Promote Youth Engagement",
				principleDescription:
					"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis excepturi labore similique repellat aspernatur? Cumque corrupti quod debitis et ex illum, eum ducimus totam blanditiis eius, natus deserunt nesciunt veritatis?",
				outcome:
					"Youth engagement and advocacy development to inspire collective intergenerational action",
				outcomeDescription:
					"Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis excepturi labore similique repellat aspernatur? Cumque corrupti quod debitis et ex illum, eum ducimus totam blanditiis eius, natus deserunt nesciunt veritatis?",
			},
		],
	}),
	methods: {
		next() {
			this.onboarding =
				this.onboarding + 1 === this.length ? 0 : this.onboarding + 1;
		},
		prev() {
			this.onboarding =
				this.onboarding - 1 < 0 ? this.length - 1 : this.onboarding - 1;
		},
	},
	components: { SlidesItem },
};
</script>
