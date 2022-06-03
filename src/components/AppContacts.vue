<template>
  <section>
    <div class="container">
      <div class="text">
        <div class="title">Contact with our team</div>
        <div class="small-text">
          If you are planning on developing a product landing
        </div>
      </div>
      <div class="localisation">
        <div class="map">
          <img src="../assets/img/StaticMapService.GetMapIma.png" alt="" />
          <div class="indication">
            <div class="indication__text">
              <div class="location">Store Avey</div>
              <div class="street">San Francisco, California 94129</div>
              <div class="map-link">
                <a href="">Visualizza mappa più grande</a>
              </div>
            </div>
            <div class="indication__icon">
              <img class="arrow" src="../assets/img/arrow.png" alt="" />
              <div class="icon-text">indicazi...</div>
            </div>
          </div>
          <div class="localisator">
            <img src="../assets/img/map-localisator.png" alt="" />
          </div>
          <div class="zoom">
            <div class="plus">
              <a href=""><i class="fas fa-plus"></i></a>
            </div>
            <div class="minus">
              <a href=""><i class="fas fa-minus"></i></a>
            </div>
          </div>
        </div>
        <div class="adress">
          <div class="logo">
            <img src="../assets/img/35.png" alt="" />
          </div>
          <div class="adress-street">9840 Shore St. Fond Du Lac, WI 54935</div>
          <div class="phone-number">0 1223 456 789</div>
          <div class="mail">mail@sofbox.com</div>
          <div class="social-icons">
            <div class="button facebook">
              <i class="fab fa-facebook-f fa-2x"></i>
            </div>
            <div class="button twitter">
              <i class="fab fa-twitter fa-2x"></i>
            </div>
            <div class="button github">
              <i class="fab fa-github fa-2x"></i>
            </div>
            <div class="button instagram">
              <i class="fab fa-instagram fa-2x"></i>
            </div>
          </div>
          <div class="contacts">
            <div class="contacts__title">Get in Touch</div>
            <div class="name-mail">
              <div class="name-input">
                <input type="text" placeholder="Your Name" />
              </div>
              <div class="mail-input">
                <input type="text" placeholder="Your Mail" />
              </div>
            </div>
            <div class="subject">
              <input type="text" placeholder="Your Subject" />
            </div>
            <div class="message">
              <textarea
                name=""
                id=""
                cols="30"
                rows="10"
                placeholder="Your Message"
              ></textarea>
            </div>
            <div class="myButton">Send Message</div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AppContacts",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/socialIcons.scss";

@import "../assets/style/variables.scss";
section {
  .text {
    text-align: center;
    margin-bottom: 4rem;
    .title {
      font-size: 30px;
      padding-bottom: 1rem;
    }
    .small-text {
      font-size: 12px;
      color: $text-color06;
    }
  }
  .localisation {
    display: flex;
    .map {
      width: calc(100% / 2 - 2rem);
      height: 50%;
      position: relative;
      margin-right: 1rem;
      .indication {
        display: flex;
        justify-content: space-between;
        position: absolute;
        top: 0;
        background-color: white;
        padding: 7px;
        margin: 10px;
        &__text {
          margin-right: 2rem;
          .location {
            font-size: 15px;
            font-weight: 500;
          }
          .street {
            font-size: 12px;
            color: $text-color04;
            margin-bottom: 1rem;
          }
          .map-link a {
            font-size: 12px;
            color: $text-color05;
            font-weight: 500;
          }
        }
        &__icon {
          text-align: center;
          height: 60%;
          .arrow {
            width: 20px;
            opacity: 50%;
          }
          .icon-text {
            font-size: 12px;
            color: $text-color05;
            font-weight: 500;
          }
        }
      }
      .localisator img {
        width: 30px;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
      }
      .zoom {
        display: flex;
        flex-direction: column;
        align-items: center;
        border: 0.5px solid lightgray;
        position: absolute;
        bottom: 10px;
        right: 0;
        background: white;
        margin: 10px;
        padding: 8px;

        .plus i {
          border-bottom: 1px solid gray;
          padding: 5px;
          color: gray;
          font-weight: bold;
        }
        .minus i {
          color: gray;
          padding: 5px;
          font-weight: bold;
        }
      }
    }
    .adress {
      .logo {
        width: 100px;
        margin-bottom: 2rem;
      }
      .adress-street {
        font-weight: 500;
        margin-bottom: 1rem;
      }
      .phone-number {
        font-size: 12px;
        color: $text-color04;
        margin-bottom: 0.5rem;
      }
      .mail {
        font-size: 12px;
        color: $text-color04;
      }
      .social-icons {
        width: 50%;
        display: flex;
        font-size: 8px;
        justify-content: space-around;
        margin: 3rem 0 2.5rem;
        color: $text-color05;
      }
      .contacts {
        input {
          padding: 10px 5px;
          border: 0.5px solid $border-color02;
        }
        &__title {
          font-weight: 500;
          margin-bottom: 1em;
        }
        .name-mail {
          display: flex;
          margin-bottom: 2rem;
          .name-input {
            margin-right: 2rem;
          }
        }
        .subject input {
          width: 100%;
          margin-bottom: 2rem;
        }
        .message textarea {
          width: 100%;
          padding: 10px 5px;
          border: 0.5px solid $border-color02;
          margin-bottom: 1rem;
        }
      }
    }
  }
}
</style>