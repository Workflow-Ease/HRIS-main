<template>
	<div class="col-lg-3 col-md-6 col-12">
		<div class="mb-4 card">
			<div class="p-3 card-body">
				<div class="d-flex flex-row-reverse justify-content-between">
					<div></div>
					<div class="contentClass">
						<div class="numbers">
							<p class="mb-0 text-sm text-uppercase font-weight-bold">연차자</p>
							<div>
								<h5 class="font-weight-bolder">{{ annualLeaveCountToday }}</h5>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>

	<div class="col-lg-3 col-md-6 col-12">
		<div class="mb-4 card">
			<div class="p-3 card-body">
				<div class="d-flex flex-row-reverse justify-content-between">
					<div></div>
					<div class="contentClass">
						<div class="numbers">
							<p class="mb-0 text-sm text-uppercase font-weight-bold">2</p>
							<div>
								<h5 class="font-weight-bolder"></h5>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>

	<div class="col-lg-3 col-md-6 col-12">
		<div class="mb-4 card">
			<div class="p-3 card-body">
				<div class="d-flex flex-row-reverse justify-content-between">
					<div></div>
					<div class="contentClass">
						<div class="numbers">
							<p class="mb-0 text-sm text-uppercase font-weight-bold">3</p>
							<div>
								<h5 class="font-weight-bolder"></h5>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>

	<div class="col-lg-3 col-md-6 col-12">
		<div class="mb-4 card">
			<div class="p-3 card-body">
				<div class="d-flex flex-row-reverse justify-content-between">
					<div></div>
					<div class="contentClass">
						<div class="numbers">
							<p class="mb-0 text-sm text-uppercase font-weight-bold">4</p>
							<div>
								<h5 class="font-weight-bolder"></h5>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script setup>
	// import { ref, computed, onMounted } from "vue";

	// 출퇴근 기록 데이터를 담을 변수
	// const attendanceTimes = ref([]);

	// 오늘의 연차자 수를 계산하는 computed 속성
	// const annualLeaveCountToday = computed(() => {
	// 	const todayDate = getTodayDate();
	// 	return attendanceTimes.value.filter(item => item.date === todayDate && item.annualLeave).length;
	// });

	// 페이지가 로드될 때 실행되는 함수
	// onMounted(async () => {
	// 	try {
	// 		// 서버에서 출퇴근 기록 데이터를 가져옴
	// 		const response = await fetch("http://localhost:3000/attendancetime");
	// 		attendanceTimes.value = await response.json();
	// 	} catch (error) {
	// 		console.error("Error fetching data:", error);
	// 	}
	// });

	// // 오늘의 날짜를 가져오는 함수
	// function getTodayDate() {
	// 	const today = new Date();
	// 	const year = today.getFullYear();
	// 	const month = String(today.getMonth() + 1).padStart(2, "0");
	// 	const day = String(today.getDate()).padStart(2, "0");
	// 	return `${year}-${month}-${day}`;
	// }
</script>
