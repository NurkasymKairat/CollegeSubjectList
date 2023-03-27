<template>
  <div>
    <section class="header">
      <div class="container">
        <nav class="navbar navbar-expand-lg bg-body-tertiary">
          <div class="container-fluid">
            <a class="navbar-brand" href="#">Втис-231 Расписание</a>
            <button
              class="navbar-toggler"
              type="button"
              data-bs-toggle="collapse"
              data-bs-target="#navbarSupportedContent"
              aria-controls="navbarSupportedContent"
              aria-expanded="false"
              aria-label="Toggle navigation"
            >
              <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
              <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                <li class="nav-item">
                  <a class="nav-link" href="#">Понедельник</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link" href="#">Вторник</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link" href="#">Среда</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link" href="#">Четверг</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link" href="#">Пятница</a>
                </li>
              </ul>
            </div>
          </div>
        </nav>
      </div>
    </section>

    <section class="listCard">
      <div class="container">
        <ul class="list-group">
          <li class="list-group-item">{{ days[0] }}</li>
          <li class="list-group-item">
            {{ subject[1] }}
            {{ numberCabs.cab122 }}
            {{ timeSub[11] }}
          </li>
          <li class="list-group-item">
            {{ subject[2] }} {{ numberCabs.cab102 }} {{ timeSub[12] }}
          </li>
          <li class="list-group-item">
            {{ subject[2] }} {{ numberCabs.cab102 }} {{ timeSub[13] }}
          </li>
          <li class="list-group-item">{{ subject[3] }} {{ timeSub[14] }}</li>
          <li class="list-group-item">
            {{ subject[9] }} {{ numberCabs.cab102 }} {{ timeSub[15] }}
          </li>
          <li class="list-group-item">
            {{ subject[9] }} {{ numberCabs.cab102 }} {{ timeSub[16] }}
          </li>
          <li class="list-group-item">
            {{ subject[6] }} {{ numberCabs.cab102 }} {{ timeSub[17] }}
          </li>
          <li class="list-group-item">
            {{ subject[4] }} {{ numberCabs.cab102 }} {{ timeSub[18] }}
          </li>
        </ul>

        <ul class="list-group">
          <li class="list-group-item">{{ days[1] }}</li>
          <li class="list-group-item">
            {{ subject[2] }} {{ numberCabs.cab110 }} {{ timeSub[11] }}
          </li>
          <li class="list-group-item">
            {{ subject[2] }} {{ numberCabs.cab110 }} {{ timeSub[12] }}
          </li>
          <li class="list-group-item">
            {{ subject[2] }} {{ numberCabs.cab110 }} {{ timeSub[13] }}
          </li>
          <li class="list-group-item">
            {{ subject[2] }} {{ numberCabs.cab110 }} {{ timeSub[14] }}
          </li>
          <li class="list-group-item">
            {{ subject[9] }} {{ numberCabs.cab110 }} {{ timeSub[15] }}
          </li>
          <li class="list-group-item">
            {{ subject[4] }} {{ numberCabs.cab110 }} {{ timeSub[16] }}
          </li>
          <li class="list-group-item">
            {{ subject[5] }} {{ numberCabs.cab122 }} {{ timeSub[17] }}
          </li>
          <li class="list-group-item">
            {{ subject[5] }} {{ numberCabs.cab122 }} {{ timeSub[18] }}
          </li>
        </ul>

        <ul class="list-group">
          <li class="list-group-item">{{ days[2] }}</li>
          <li class="list-group-item"></li>
          <li class="list-group-item">
            {{ subject[6] }} {{ numberCabs.cab122 }} {{ timeSub[13] }}
          </li>
          <li class="list-group-item">
            {{ subject[6] }} {{ numberCabs.cab122 }} {{ timeSub[14] }}
          </li>
          <li class="list-group-item">
            {{ subject[6] }} {{ numberCabs.cab122 }} {{ timeSub[15] }}
          </li>
          <li class="list-group-item">
            {{ subject[7] }} {{ numberCabs.cab122 }} {{ timeSub[16] }}
          </li>
          <li class="list-group-item">
            {{ subject[7] }} {{ numberCabs.cab122 }} {{ timeSub[17] }}
          </li>
          <li class="list-group-item">
            {{ subject[7] }} {{ numberCabs.cab122 }} {{ timeSub[18] }}
          </li>
        </ul>

        <ul class="list-group">
          <li class="list-group-item">{{ days[3] }}</li>
          <li class="list-group-item">
            {{ subject[1] }} {{ numberCabs.cab301 }} {{ timeSub[10] }}
          </li>
          <li class="list-group-item">
            {{ subject[1] }} {{ numberCabs.cab112 }} {{ timeSub[11] }}
          </li>
          <li class="list-group-item">
            {{ subject[2] }} {{ numberCabs.cab101 }} {{ timeSub[12] }}
          </li>
          <li class="list-group-item">
            {{ subject[2] }} {{ numberCabs.cab110 }} {{ timeSub[13] }}
          </li>
          <li class="list-group-item">
            {{ subject[4] }} {{ numberCabs.cab306 }} {{ timeSub[14] }}
          </li>
          <li class="list-group-item">
            {{ subject[4] }} {{ numberCabs.cab103 }} {{ timeSub[15] }}
          </li>
          <li class="list-group-item">
            {{ subject[8] }} {{ numberCabs.cab103 }} {{ timeSub[16] }}
          </li>
          <li class="list-group-item">
            {{ subject[8] }} {{ numberCabs.cab301 }} {{ timeSub[17] }}
          </li>
        </ul>

        <ul class="list-group">
          <li class="list-group-item">{{ days[4] }}</li>
          <li class="list-group-item">
            {{ subject[9] }} {{ numberCabs.cab205 }} {{ timeSub[11] }}
          </li>
          <li class="list-group-item">
            {{ subject[4] }} {{ numberCabs.cab110 }} {{ timeSub[12] }}
          </li>
          <li class="list-group-item">
            {{ subject[1] }} {{ numberCabs.cab110 }} {{ timeSub[13] }}
          </li>
          <li class="list-group-item">
            {{ subject[4] }} {{ numberCabs.cab108 }} {{ timeSub[14] }}
          </li>
          <li class="list-group-item">
            {{ subject[5] }} {{ numberCabs.cab122 }} {{ timeSub[15] }}
          </li>
          <li class="list-group-item">
            {{ subject[5] }} {{ numberCabs.cab122 }} {{ timeSub[16] }}
          </li>
          <li class="list-group-item">
            {{ subject[7] }} {{ numberCabs.cab122 }} {{ timeSub[17] }}
          </li>
          <li class="list-group-item">
            {{ subject[7] }} {{ numberCabs.cab122 }} {{ timeSub[18] }}
          </li>
        </ul>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "HeaderApp",
  data() {
    return {
      days: ["Понедельник", "Вторник", "Среда", "Четверг", "Пятница"],

      numberCabs: {
        cab122: "122",
        cab102: "102",
        cab103: "103",
        cab110: "110",
        cab101: "101",
        cab113: "113",
        cab122: "122",
        cab417: "417",
        cab108: "108",
        cab301: "301",
        cab112: "112",
        cab306: "306",
        cab203: "203",
        cab205: "205",
      },

      timeSub: {
        10: "10:35-11:20",
        11: "11:40-12:25",
        12: "12:30-13:15",
        13: "13:25-14:10",
        14: "14:15-15:00",
        15: "15:05-15:50",
        16: "16:00-16:45",
        17: "16:55-17:35",
        18: "17:45-18:30",
      },

      subject: {
        1: "Основы программирования и алгорг Бердібек М",
        2: "Архитектура компьютерных сетей ср. Бердібек М",
        3: "Физическая культура Садыбаев Е.А стадион",
        4: "Введенне в сетевые технологии Бердібек М",
        5: "Операционные системы компьютерной техни т. Кабдолла А.Р",
        6: "Аппаратное обеспечение компьютерной техи пр. Каблолла A.P",
        7: "Микросхематехника пр. Кабдолла А.Р",
        8: "Английский язык Омарова С.А",
        9: "Программное обеспечение пр. Мусина К.Р",
        10: "Arduino пр. Кенебаев А",
      },

      selectedIndex: true,

      Monday: false,
      Thuesday: false,
      Wednesday: false,
      Thertday: false,
      Friday: false,
    };
  },
  computed: {},
  methods: {
    selectDay() {
      const tabs = document.querySelectorAll(".nav-link"),
        tabItem = document.querySelectorAll(".list-group"),
        tabParent = document.querySelector(".navbar-nav");

      function hideTab() {
        tabs.forEach((item) => {
          item.classList.remove("active");
        });
        tabItem.forEach((item) => {
          item.classList.add("hide");
          item.classList.remove("show");
        });
      }

      function showItem(i = 0) {
        tabItem[i].classList.add("show");
        tabItem[i].classList.remove("hide");
        tabs[i].classList.add("active");
      }

      hideTab();

      tabParent.addEventListener("click", (e) => {
        const target = e.target;
        target.classList.contains(".nav-link");
        tabs.forEach((item, i) => {
          if (target == item) {
            hideTab();
            showItem(i);
          }
        });
      });
    },
  },
  mounted() {
    this.selectDay();
  },
};
</script>
<style lang="scss">
.listCard {
  margin-top: 30px;
  .list-group {
    transition: opacity 0.5s ease-in-out;
  }

  ul {
    margin-bottom: 30px;
  }
}

.show {
  opacity: 1;
  display: block;
}

.hide {
  display: none;
  opacity: 0;
}
</style>
