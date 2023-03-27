<template>
  <section class="footer">
    <div class="container">
      <button @click="addTrue" class="modal_btn">{{ textBtn }}</button>
      <form action="" method="POST">
        <div v-if="btnAdd" class="modal_item">
         
          <div class="modal_block">
            <input
              type="text"
              required
              placeholder="Ваше имя..."
              name="name"
              id="contact-name"
            />
            <span id="name-error"></span>
          </div>
          <div class="modal_block">
            <input
              type="text"
              required
              placeholder="Ваше сообшения"
              name="telephone"
              id="contact-phone"
            />
            <span id="phone-error"></span>
          </div>
          <div class="modal_block">
            <button required data-open class="btn" id="contact-btn">
              Отправить
            </button>
            <span id="sub-error"></span>
          </div>
        </div>
      </form>

      <div class="footer_info">© 2023</div>
    </div>
  </section>
</template>
<script>
export default {
  name: "FooterApp",
  data() {
    return {
      btnAdd: false,
      textBtn: 'Оставьте отзыв',
    }
  },
  methods: {
    addTrue() {
      if (this.btnAdd !== true) {
        this.btnAdd = true;
        this.textBtn = 'Закрыть'
      } else {
        this.btnAdd = false;
        this.textBtn = 'Оставьте отзыв'
      }
    }
  }
};
</script>
<style lang="scss">
.footer { 
    text-align: right;
  &_info {
    opacity: 0.9;
    font-size: 13px;
    line-height: 17px;
    font-weight: 300;
    color: #000000;
  }

  .modal {
    &_item {
      text-align: right;
    }

    &_btn {
      margin-bottom: 5px;
      padding: 10px 20px;
      background-color: #eb7070;
      font-weight: 400;
      font-size: 15px;
      color: #fff;
      outline: none;
      border: none;
      border-radius: 15px;
    }

    &_block {
      position: relative;
      text-align: right;
      margin: 20px auto;
      display: block;
      margin-right: 30px;
      input {
        width: 250px;
        border-radius: 30px;
        padding-left: 20px;
        height: 47px;
        background-color: #ffffff;
        border: 1px solid rgba(0, 0, 0, 0.2);
        font-size: 13px;
        line-height: 24px;
        font-weight: 300;
        color: #101010;
        outline: none;
      }
      button {
        margin: 0;
        padding: 10px 20px;
        background-color: #eb7070;
        font-weight: 400;
        font-size: 15px;
        color: #fff;
      }
    }
  }
}
</style>
