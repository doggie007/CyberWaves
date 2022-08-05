<template>
	<v-window-item>
		<v-card outlined>
			<v-list-item>
				<v-list-item-content>
					<div>
						<div class="text-overline text-capitalize mb-2">
							Problem {{ number + 1 }}
						</div>
						<v-list-item-title class="text-h5 text-md-h4 py-4 text-wrap">
							{{ item.issue }}
						</v-list-item-title>
						<v-list-item-subtitle class="text-wrap text-md-body-1">{{
							item.issueDescription
						}}</v-list-item-subtitle>
					</div>
					<div>
						<v-icon class="mt-4" large> mdi-arrow-down </v-icon>
					</div>
					<v-divider></v-divider>
					<div>
						<div class="text-overline text-capitalize mt-4 mb-2">
							Principle {{ number + 1 }}
						</div>
						<v-list-item-title
							class="text-h5 text-md-h4 text-md-h4 py-4 text-wrap"
						>
							{{ item.principle }}
						</v-list-item-title>
						<v-list-item-subtitle class="text-wrap text-md-body-1">{{
							item.principleDescription
						}}</v-list-item-subtitle>
					</div>
					<div>
						<v-icon class="mt-4" large> mdi-arrow-down </v-icon>
					</div>
					<v-divider></v-divider>
					<div>
						<div class="text-overline text-capitalize mt-4 mb-2">
							Outcome {{ number + 1 }}
						</div>
						<v-list-item-title class="text-h5 text-md-h4 py-4 text-wrap">
							{{ item.outcome }}
						</v-list-item-title>
						<v-list-item-subtitle class="text-wrap text-md-body-1">{{
							item.outcomeDescription
						}}</v-list-item-subtitle>
					</div>
					<div class="py-4"></div>
				</v-list-item-content>
			</v-list-item>
		</v-card>
	</v-window-item>
</template>
<script>
export default {
	props: {
		item: Object,
		number: Number,
	},
};
</script>
