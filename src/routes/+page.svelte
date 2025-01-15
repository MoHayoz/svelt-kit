<script>
    let donationAmount = "";
  
    function handleDonate() {
      alert(`Vielen Dank für Ihre Spende von ${donationAmount} CHF!`);
      donationAmount = "";
    }
  </script>
  
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: url('https://static.spektrum.de/fm/912/f2000x857/iStock-910488902_quer.jpg') no-repeat center center/cover;
      color: white;
      overflow: hidden;
    }
  
    .container {
      background: rgba(0, 0, 0, 0.7);
      padding: 2rem;
      border-radius: 10px;
      text-align: center;
      width: 100%;
      max-width: 600px;
      margin: 0 auto;
    }
  
    h1 {
      margin-bottom: 1rem;
    }
  
    p {
      margin-bottom: 1.5rem;
      line-height: 1.6;
    }
  
    .donation-section {
      margin-top: 1rem;
    }
  
    input {
      padding: 0.5rem;
      border: none;
      border-radius: 4px;
      margin-right: 0.5rem;
      width: 150px;
    }
  
    button {
      padding: 0.5rem 1rem;
      background-color: #3498db;
      color: white;
      border: none;
      border-radius: 4px;
      cursor: pointer;
    }
  
    button:hover {
      background-color: #2980b9;
    }
  </style>
  
  <div class="container">
    <h1>Spenden für Hoffnung-Auragen</h1>
    <p>
      Unterstützen Sie unsere Mission, Hoffnung und Heilung für Betroffene der
      Auragen-Dystrophie zu bringen. Jedes Jahr kämpfen Tausende Menschen mit
      dieser seltenen Krankheit. Gemeinsam können wir die Forschung fördern,
      Therapien entwickeln und das Leben der Betroffenen verbessern.
    </p>
    <div class="donation-section">
      <input
        type="number"
        min="1"
        placeholder="Betrag in CHF"
        bind:value={donationAmount}
      />
      <button on:click={handleDonate}>Jetzt spenden</button>
    </div>
  </div>
  
