<template>
  <div class="join">
    <h1>Do you want to join our team?</h1>
    <form class="form">
      <div class="form-wrapper">
        <label for="Name">Naam</label>
        <input class="input" type="text" name="name" id="Name">
      </div>
      <div class="form-wrapper">
        <label for="FName">Voornaam</label>
        <input class="input" type="text" name="fName" id="FName">
      </div>
      <div class="form-wrapper">
        <label for="BirthDate">Geboortedatum</label>
        <input class="input" type="date" name="birthDate" id="BirthDate">
      </div>
      <div class="form-wrapper">
        <label for="Mail">E-Mail</label>
        <input class="input" type="email" name="mail" id="Mail">
      </div>
      <div class="form-wrapper">
        <label for="Phone">Telefoon nummer</label>
        <input class="input" type="text" name="phone" id="Phone">
      </div>
      <div class="form-wrapper">
        <label for="Why">Waarom jij?</label>
        <textarea class="input" name="why" id="Why"></textarea>
      </div>
      <div class="form-wrapper">
        <label for="Tasks">Welke taak wil jij?</label>
        <div class="form-radio">
          <div class="form-wrapper-rb">
            <input type="checkbox" id="Klusjes" name="rbklusjes" value="Klusjes">
            <label for="Klusjes">Klusjes</label>
          </div>
          <div class="form-wrapper-rb">
            <input type="checkbox" id="Poetsen" name="rbpoetsen" value="Poetsen">
            <label for="Poetsen">Poetsen</label>
          </div>
          <div class="form-wrapper-rb">
            <input type="checkbox" id="Inkleding" name="rbinkleding" value="Inkleding">
            <label for="Inkleding">Inkleding</label>
          </div>
          <div class="form-wrapper-rb">
            <input type="checkbox" id="Events_BTS" name="rbevents_bts" value="Evenementen bedenken en uitwerken">
            <label for="Events_BTS">Evenementen bedenken en uitwerken</label>
          </div>
          <div class="form-wrapper-rb">
            <input type="checkbox" id="Events_Buildup" name="rbevents_buildup" value="Evenementen opbouwen">
            <label for="Events_Buildup">Evenementen opbouwen</label>
          </div>
          <div class="form-wrapper-rb">
            <input type="checkbox" id="Tappen" name="rbtappen" value="Alleen tappen">
            <label for="Tappen">Alleen tappen</label>
          </div>
        </div>
      </div>
      <div class="submit">
        <input type="submit" name="submit" id="Submit" value="Submit">
      </div>
    </form>
  </div>
</template>

<style>
.join {
  background-color: #343434;
  padding: 30px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  max-width: 500px;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

h1 {
  text-align: center;
  color: #f2f2f2;
  margin-bottom: 20px;
  font-size: 24px;
}

.form {
  display: flex;
  flex-direction: column;
}

.form-wrapper {
  display: flex;
  flex-direction: column;
  margin-bottom: 15px;
}

.form-wrapper label {
  margin-bottom: 5px;
  font-weight: bold;
  color: #f2f2f2;
}

.input {
  padding: 10px;
  border-radius: 5px;
  border: 1px solid #ccc;
  font-size: 16px;
}

.input[type="text"], .input[type="email"], .input[type="date"], .input[type="textarea"] {
  width: 100%;
}

.form-radio {
  display: flex;
  flex-wrap: wrap;
}

.form-wrapper-rb {
  margin-right: 20px;
  margin-bottom: 10px;
}

.form-wrapper-rb input {
  margin-right: 5px;
}

.submit {
  display: flex;
  justify-content: center;
  margin-top: 20px;
}

.submit input {
  background-color: #216477;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 16px;
}

.submit input:hover {
  background-color: #025669;
}

@media (min-width: 768px) {
  .join {
    padding: 40px;
  }

  h1 {
    font-size: 28px;
  }

  .input {
    font-size: 18px;
  }

  .submit input {
    padding: 12px 24px;
    font-size: 18px;
  }
}
</style>

<script>

</script>
