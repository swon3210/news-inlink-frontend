<template>
  <v-container fill-height>
    <v-row
      class="flex-child ma-0"
    >
      <v-col
        class="d-flex"
        cols="12"
      >
        <v-row>
          <v-col cols="12">
            <v-sheet
              class="d-flex"
              color="white lighten-3"
              :elevation="2"
              max-height="300"
            >
              <v-img 
                src="https://imgnews.pstatic.net/image/005/2019/09/09/611220190013694742_1_20190909134404774.jpg?type=w647"
              />
            </v-sheet>
          </v-col>

          <v-col cols="12">
            <v-sheet
              color="white lighten-3"
              min-height="500"
              :elevation="2"

            >
              <h2 v-text="heading" class="pl-10 py-5"></h2>
              <v-divider></v-divider>
              <p class="pa-10" v-html="post_text">
                
              </p>
            </v-sheet>
          </v-col>
          <!-- <v-col cols="6">
            <v-sheet
              class="d-flex"
              color="green lighten-3"
              height="200"
            >
            </v-sheet>
          </v-col>
          <v-col cols="6">
            <v-sheet
              class="d-flex"
              color="yellow lighten-3"
              height="200"
            >
            </v-sheet>
          </v-col> -->
          <v-col>
            <div class="text-center">
              <v-pagination
                v-model="page"
                :length="6"
              ></v-pagination>
            </div>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
    
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      heading: `‘NO 재팬’ 부산항여객터미널과 대마도 한국상인들 피해 심각`,
      post_text: `휴일이면 수 천명이 북적이던 부산항국제여객터미널이 휴일인 8일 오후 승객들이 없어 직원 몇명만 자리를 지키고 있다
<br />
<br />
일본 제품 불매 운동이 장기화되면서 부산항국제여객선터미널과 대마도 내 한국상인들의 피해가 심각한 것으로 나타났다.
<br /><br />

9일 부산시와 부산항만공사 등에 따르면 부산과 일본을 오가는 여객이 두 달여 만에 20% 수준으로 급감, 부산항국제여객터미널이 운영에 어려움을 겪고 있다.
<br /><br />

일본을 오가는 이용객이 크게 줄면서 대마도를 오가는 배편 중 특정 지역은 아예 끊기는 등 한일 항로 운항 자체가 존폐 기로에 놓였다.
<br /><br />

인기가 높았던 부산~대마도 배편은 하루 6척에서 2척만 남았다. 부산에서 대마도 이즈하라항으로 가는 4척의 배편은 지난달 19일 이후 모두 끊겼고, 대아고속해운은 부산~대마도 히타카쓰항 노선을 스타라인과 격일제로 2척을 번갈아 운항하고 있다.
<br /><br />

부산항국제여객터미널 관계자는 “지난 6월까지만 해도 일요일 운항 선박이 많을 때는 15척에 달했는데 최근 2척만 운항된다”며 “이용객도 6월에는 6000명이 넘었지만 최근 600~700명으로 급감했다”고 말했다.
<br />
<br />

부산항국제여객터미널 내 식당가도 손님이 없어 휴업을 준비하고 있다
<br />
<br />

이 때문에 터미널 내 식당과 카페 등은 개점휴업 상태다. 식당가에는 세관 직원과 여객선사 직원 몇 명이 이용하는 정도다. 식당 관계자는 “6월까지 하루 500여명의 손님이 찾았는데 최근에는 20~30명밖에 안된다”며 한숨지었다.
<br /><br />

또 터미널 순환버스 운영사는 일본 여행객 급감 여파로 휴업을 검토 중인 것으로 알려졌다.
<br /><br />

업체 관계자는 “최근 승객 수가 3분의 1수준으로 급감했다”며 “차량 유지비, 유류비, 기사 인건비 등으로 월 700만원 이상의 적자가 발생해 더 이상 운영이 어렵다”는 입장을 보였다.
<br /><br />

시와 부산항만공사 관계자는 “터미널 입주업체들에게 임대료 납부 유예 등의 대책을 제안했지만 영업 중단 의사를 밝히는 업체들이 늘고 있다”며 “업계 피해를 최소화할 수 있는 방안을 찾기 위해 노력하고 있다”고 말했다.
<br /><br />

이와 함께 비자를 받아 대마도에서 영업을 하는 한국인들의 피해도 심각한 것으로 알려졌다.
<br />
부산~대마도 간을 오가며 영업하는 여행가이드 A씨(40)는 “대마도에서 관광버스, 호텔, 민박, 낚시, 식당, 자전거대여 등을 하는 상인들의 90%가 한국인”이라며 “최근 두달 여 동안 이들 업체 대부분이 직원들을 해고하고 폐업한 상태”라고 말했다.
<br /><br />

대마도에서 식당 등을 운영하는 B씨(60)는 “최근 직원 30명을 퇴사 시키고 영업을 잠정 중단했다”고 말했다.
<br /><br />

대마도 관광객들이 줄면서 연간 35만여명을 상대로 영업하던 여행가이드 수 천명도 일자리를 잃은 것으로 알려졌다.
<br /><br />

<br />
부산=윤봉학 기자 bhyoon@kmib.co.kr

<br /><br />

GoodNews paper ⓒ 국민일보(www.kmib.co.kr), 무단전재 및 재배포금지`,
      page: 1,
    }
  },
  components: {

  }
}
</script>
