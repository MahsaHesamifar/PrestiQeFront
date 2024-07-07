<template>
  <v-container class="pa-0" fluid>
    <v-row align="center" class="test mx-16 px-16">
      <v-col>
        <div class="text-center pb-5" style="font-size: 3rem">
          ثبت نام<br />
        </div>
        <v-form v-model="valid">
          <v-text-field
            label="شماره همراه"
            variant="outlined"
            v-model="phoneNumber"
            rounded
          ></v-text-field>
          <v-text-field
            label="نام کاربری"
            variant="outlined"
            v-model="userName"
            rounded
          ></v-text-field>

          <v-text-field
            v-model="password"
            variant="outlined"
            :append-inner-icon="show1 ? 'mdi-eye' : 'mdi-eye-off'"
            :rules="[rules.required]"
            :type="show1 ? 'text' : 'password'"
            label="رمز عبور"
            rounded
            @click:appendInner="show1 = !show1"
          ></v-text-field>
          <v-text-field
            v-model="password"
            variant="outlined"
            :append-inner-icon="show1 ? 'mdi-eye' : 'mdi-eye-off'"
            :rules="[rules.required]"
            :type="show1 ? 'text' : 'password'"
            label="تکرار رمز عبور"
            rounded
            @click:appendInner="show1 = !show1"
          ></v-text-field>
          <v-btn
            class="gdBg text-h6"
            style="
              background: linear-gradient(
                303deg,
                rgba(250, 139, 255, 1) 7%,
                rgba(43, 210, 255, 1) 47%,
                rgba(43, 255, 136, 1) 83%
              );
              color: black;
              padding: 4vh 0vh;
            "
            rounded
            block
            @click="validate"
          >
            ثبت نام
          </v-btn>
        </v-form>
        <v-row>
          <v-col>
            <v-btn variant="text" color=" rgb(129, 129, 129)"
              >حساب کاربری دارید</v-btn
            >
          </v-col>
          <v-col
            ><v-btn
              variant="text"
              color="#FF57F8"
              style="margin-right: 10vw"
              class="text-decoration-underline"
              >ورود</v-btn
            ></v-col
          >
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      show1: false,
      show2: true,
      password: "",
      userName: "",
      rules: {
        required: (value) => !!value || "اجباری",
      },
    };
  },
};
</script>

<style>
.test {
  height: 105vh;
}
.gdBg {
  margin: 2vh 0vh;
}
</style>
