<template>
  <div class="contactmain animated fadeIn">
    <div class="anyquestions">
      <br>
      <br>
      <p style="font-size:1.5rem;">FOR ANY QUESTIONS, PLEASE CALL OR EMAIL US. ALTERNATIVELY, YOU CAN FILL IN THE FOLLOWING CONTACT FORM.</p>
      <div class="infobox2">
        <br>
        <p>20 Floral Parkway</p>
        <p>Concord, ON L4K 4R1</p>
        <br>
        <p>Tel: 905-695-1424</p>
        <p>info@ozzev.com</p>
        <br>
        <p>Follow Us:</p>
        <p>
          <!--<img src="/img/googleplus.png" alt="googleplus"/>-->
          <img src="/img/linkedin.png" alt="linkedin"/></p>
        <br>
        <p>© 2019 by OZZ EV Inc. All rights reserved.</p>
        <br>
        <br>
      </div>
    </div>
    <div class="contactform">
        <div class="content">
          <form name="contact" method="POST" data-netlify="true">
            <input type="hidden" name="form-name" value="contact"/>

            <p>
              <!--<label class="form-label" for="name">NAME:</label>-->
              <input class="form-field" type="text" name="name" id="name" placeholder="NAME*"/>
            </p>

            <p>
                <!--<label class="form-label" for="email">EMAIL:</label>-->
                <input class="form-field" type="email" name="email" id="email" placeholder="EMAIL*" />
            </p>

            <!--<p>-->
                <!--&lt;!&ndash;<label class="form-label" for="subject">SUBJECT:</label>&ndash;&gt;-->
                <!--<input class="form-field" name="subject" id="subject" placeholder="SUBJECT" />-->
            <!--</p>-->

            <p>
                <!--<label class="form-label" for="message">MESSAGE:</label>-->
                <textarea class="form-field" name="message" id="message" placeholder="MESSAGE*"></textarea>
            </p>

            <p class="hidden">
              <label>Don't fill this out: <input name="bot-field"></label>
            </p>

            <p><input class="form-button" type="submit" value="SEND MESSAGE" /></p>
          </form>
        </div>
    </div>
  </div>
</template>

<style>
  input {
    width:100%;
    /*box-sizing: border-box;*/
    font-size: 1rem;
    background-color: rgba(141,143,155,1);
    padding: 1%;
    color: white;
    margin: 3%;
    border: none
  }

  input::placeholder {
    font-size: .75rem;
    color: white;
    font-family: "Brandon-Grotesque-bold";
  }

  input[type=submit] {
    font-size: .75rem;
    color: black !important;
    font-family: "Brandon-Grotesque-bold";
  }

  textarea {
    width:100%;
    /*box-sizing: border-box;*/
    font-size: 1rem;
    background-color: rgba(141,143,155,1);
    padding: 1%;
    color: white;
    margin: 3%;
    height: 6rem;
    border: none;
  }

  textarea::placeholder {
    font-size: .75rem;
    color: white;
    font-family: "Brandon-Grotesque-bold";
  }

</style>
