# fraces.SCRIPT
const quotes = [
  { text: "El éxito es la suma de pequeños esfuerzos repetidos día tras día.", author: "Robert Collier" },
  { text: "La mejor manera de predecir el futuro es crearlo.", author: "Peter Drucker" },
  { text: "No cuentes los días, haz que los días cuenten.", author: "Muhammad Ali" },
  { text: "El único límite para nuestros logros de mañana son nuestras dudas de hoy.", author: "Franklin D. Roosevelt" },
  { text: "Cree en ti mismo y todo será posible.", author: "Anónimo" }
];

function generateQuote() {
  const randomIndex = Math.floor(Math.random() * quotes.length);
  const quote = quotes[randomIndex];
  document.getElementById('quote').innerText = quote.text;
  document.getElementById('author').innerText = `- ${quote.author}`;
}
