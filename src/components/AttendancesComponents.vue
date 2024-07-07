<template>
  <v-container class="pa-0" fluid>
    <v-row align="center" class="test mx-16 px-16">
      <v-col>
        <v-container class="attendance-style">
          <div class="header">
            <span class="title">لیست شرکت کنندگان</span>
            <button class="close-btn" @click="closeList">✖</button>
          </div>
          <div class="participants">
            <div
              v-for="participant in participants"
              :key="participant.id"
              class="participant"
            >
              <img :src="participant.image" alt="avatar" class="avatar" />
              <div class="info">
                <span class="name">{{ participant.name }}</span>
                <span class="level">LVL {{ participant.level }}</span>
              </div>
              <button class="view-profile-btn">مشاهده پروفایل</button>
            </div>
          </div>
        </v-container>
      </v-col>
    </v-row>
  </v-container>
</template>

<style>
.test {
  height: 105vh;
}
.gdBg {
  margin: 2vh 0vh;
}
.attendance-style {
  height: 75vh;
  background-color: #21263d;
  border-radius: 2vw;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 0;
}

.title {
  font-size: 1.5vw;
  font-weight: bold;
  color: #5d688d;
  margin: 0 auto;
}

.close-btn {
  background: none;
  border: none;
  color: #5d688d;
  font-size: 20px;
  cursor: pointer;
}

.participants {
  max-height: 58vh;
  overflow-y: auto;
  direction: ltr;
  overflow-y: scroll;
  scrollbar-color: #616d92 #2f354f;
  scrollbar-width: thin;
}

.participant {
  display: flex;
  align-items: center;
  padding: 10px 0;
  border-bottom: 1px solid #3e4a5b;
}

.avatar {
  width: 40px;
  height: 40px;
  border-radius: 0.5vi;
  margin: 0 10px;
}

.info {
  flex-grow: 1;
}

.name {
  display: block;
  font-size: 14px;
  font-weight: bold;
}

.level {
  display: block;
  font-size: 12px;
  color: #5d688d;
}

.view-profile-btn {
  background-color: #21263d;
  color: #2bd2ff;
  padding: 8px 12px;
  border: 1px solid #2bd2ff;
  border-radius: 5px;
  font-family: Dubai;
  font-size: 12px;
  margin-right: 4px;
}
</style>

<script>
export default {
  data() {
    return {
      participants: [
        {
          id: 1,
          name: "Roberto Salbado",
          level: 15,
          image:
            "https://protoinfrastack-myfirstbucketb8884501-fnnzvxt2ee5v.s3.amazonaws.com/mgIzZFlF08R0g5QcU2azAFGYx8KTSeiBOENk",
        },
        {
          id: 2,
          name: "XenonPhoenix",
          level: 8,
          image:
            "https://protoinfrastack-myfirstbucketb8884501-fnnzvxt2ee5v.s3.amazonaws.com/mgIzZFlF08R0g5QcU2azAFGYx8KTSeiBOENk",
        },
        {
          id: 3,
          name: "toxic girl",
          level: 2,
          image:
            "https://protoinfrastack-myfirstbucketb8884501-fnnzvxt2ee5v.s3.amazonaws.com/mgIzZFlF08R0g5QcU2azAFGYx8KTSeiBOENk",
        },
        {
          id: 4,
          name: "toxic girl",
          level: 2,
          image:
            "https://protoinfrastack-myfirstbucketb8884501-fnnzvxt2ee5v.s3.amazonaws.com/mgIzZFlF08R0g5QcU2azAFGYx8KTSeiBOENk",
        },
        {
          id: 5,
          name: "toxic girl",
          level: 2,
          image:
            "https://protoinfrastack-myfirstbucketb8884501-fnnzvxt2ee5v.s3.amazonaws.com/mgIzZFlF08R0g5QcU2azAFGYx8KTSeiBOENk",
        },
        {
          id: 6,
          name: "toxic girl",
          level: 2,
          image:
            "https://protoinfrastack-myfirstbucketb8884501-fnnzvxt2ee5v.s3.amazonaws.com/mgIzZFlF08R0g5QcU2azAFGYx8KTSeiBOENk",
        },
        {
          id: 7,
          name: "toxic girl",
          level: 1,
          image:
            "https://protoinfrastack-myfirstbucketb8884501-fnnzvxt2ee5v.s3.amazonaws.com/mgIzZFlF08R0g5QcU2azAFGYx8KTSeiBOENk",
        },
        {
          id: 8,
          name: "toxic girl",
          level: 3,
          image:
            "https://protoinfrastack-myfirstbucketb8884501-fnnzvxt2ee5v.s3.amazonaws.com/mgIzZFlF08R0g5QcU2azAFGYx8KTSeiBOENk",
        },
      ],
    };
  },
  methods: {
    closeList() {
      // Implement the logic to close the participant list
    },
  },
};
</script>
