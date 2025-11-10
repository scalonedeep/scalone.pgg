<html lang="es">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Razones por las que amo a mi cachorrita</title>
<style>
body{
  margin:0;
  padding:0;
  font-family: Arial, Helvetica, sans-serif;
  background: linear-gradient(120deg,#ffd6e8,#b5f6ff);
  display:flex;
  justify-content:center;
  align-items:center;
  height:100vh;
}
.container{
  background:#ffffffcc;
  padding:30px;
  border-radius:15px;
  box-shadow:0 6px 20px rgba(0,0,0,0.1);
  text-align:center;
  width:90%;
  max-width:600px;
}
h1{
  margin-bottom:20px;
  font-size:1.8em;
  color:#ff5c8a;
}
#reason{
  font-size:1.2em;
  font-weight:bold;
  color:#222;
  background:rgba(255,255,255,0.7);
  padding:20px;
  border-radius:10px;
  min-height:100px;
  display:flex;
  align-items:center;
  justify-content:center;
  margin-bottom:20px;
}
button{
  background-color:#ff5c8a;
  color:white;
  border:none;
  padding:10px 20px;
  border-radius:8px;
  cursor:pointer;
  font-weight:bold;
}
button:hover{
  background-color:#ff7fa5;
}
</style>
</head>
<body>
<div class="container">
<h1>Razones por las que amo a mi cachorrita</h1>
<div id="reason"></div>
<button id="nextBtn">Otra razón</button>
</div>
<script>
let razones = [
  "Me encanta tu personalidad mall",
  "Tus bromas",
  "Tu manera de hablar",
  "Sos ree linda",
  "Tu calma",
  "Tu amabilidad",
  "Tu empatía",
  "Que sos re inteligente",
  "Tu forma de querer",
  "Que me haces mejor como persona",
  "Sos ree divertida",
  "Tus formas de solucionar problemas",
  "Tu curiosidad",
  "Tu humor",
  "Sos ree familiar",
  "Sos tremenda tronca y quien no ama a las troncas dea",
  "Tu intensidad",
  "Me entendés",
  "Me escuchás",
  "Cómo ves la vida",
  "Cómo sos",
  "Tu honestidad (aunque cuesta que me la digas a la primera)",
  "Tu calidez flow",
  "Tenés buenos gustos de música",
  "Me haces feliz cuando estoy mall",
  "Tus logros",
  "Tu respeto",
  "Cómo te llevas todo a la boca porque yo también lo hago",
  "Que te hagas la difícil",
  "Tus te amo",
  "Tus te extraño",
  "Sos re sumisa dea",
  "Cómo sos empalagosa conmigo",
  "Eres cuidadosa",
  "Detallista",
  "Amás al el goldo",
  "Cómo pensás con lógica",
  "Tu pensamiento crítico",
  "Cómo me alegras los días",
  "Que siempre pensás en positivo",
  "Tenés buena memoria",
  "Tus te amo",
  "Cómo me amás",
  "Tus perdón",
  "Tus bro",
  "Que sos el ana de mi shei",
  "Que te gusta coscu",
  "Que te gusta momo",
  "Cómo me das atención",
  "Cómo me aconsejás",
  "Cómo sabés lo que me gusta",
  "Porque me haces sentir importante",
  "Porque tenés un corazón gigante dea",
  "Porque te gustan los nenes chicos",
  "Porque sos ree tierna cuando eras chica",
  "Porque me haces olvidar todo lo malo",
  "Porque me das razones para sonreír dea como lo decía",
  "Porque me amás como soy",
  "Porque me haces creer que el amor trae cosas más buenas que malas",
  "Porque me haces sentir libre",
  "Porque me siento valorado",
  "Tus te adoro",
  "Tus te aprecio",
  "Porque te sueño todos los días",
  "Porque te necesito",
  "Porque sabés cocinar",
  "Porque me siento comprendido",
  "Porque me das ganas de estar a tu lado y creer con vos... me explico?",
  "Porque entendés mis estupideces",
  "Porque me siento afortunado",
  "Tenés tremenda ternura a veces",
  "Porque sos mi perrita",
  "Tu comprensión a todo",
  "Cómo te gusta hacerme feliz",
  "Porque me tenés sonriéndole al celu",
  "Tus sueños",
  "Cómo pensás en el futuro",
  "Tu orgullo",
  "Cómo la vivís en el liceo",
  "Tu forma de seguir adelante",
  "Que sos muy cómica",
  "Tus imperfecciones",
  "Te amo, no sé qué poner",
  "Te gusta Anuel",
  "Sos ree sociable",
  "Cómo querés a la gente",
  "Tu olor",
  "Tu mirada (cuando me mirás)",
  "Tus audios",
  "Que sos ree única",
  "Cómo no te importa lo que diga la gente",
  "Cómo sos vos con todos flow, me explico?",
  "Porque me das amor",
  "Tenés tremendo pelo",
  "Tu sonrisa",
  "Cómo sos ree cariñosa mall",
  "Cómo cuidás a tu hermano",
  "Cómo te pones nerviosa por todo",
  "Que seas ok",
  "Tus mi vida",
  "Cómo me decís amor",
  "Cómo decís dea",
  "Cómo pensás en el futuro",
  "Tenés tremendos stikers",
  "Que creés que me ganás en todo pero no",
  "Cómo le llenas de amor todo"
];

let texto = document.getElementById('reason');
let boton = document.getElementById('nextBtn');
let usados = new Set();

function razonRandom(){
  if(usados.size === razones.length){
    usados.clear();
  }
  let i;
  do{
    i = Math.floor(Math.random() * razones.length);
  }while(usados.has(i));
  usados.add(i);
  return razones[i];
}

boton.addEventListener('click', ()=>{
  texto.textContent = razonRandom();
});
</script>
</body>
</html>
