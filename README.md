# tarea

function estadisticasPesos() {
  let pesos = []; // arreglo para almacenar los pesos
  let menosDe40 = 0;
  let entre40y50 = 0;
  let entre50y60 = 0;
  let masDe60 = 0;

  // ingreso de pesos
  for (let i = 1; i <= 10; i++) {
    let peso = prompt(`Ingrese el peso del alumno ${i}:`);
    pesos.push(parseFloat(peso));
  }

  // clasificación de pesos
  for (let i = 0; i < pesos.length; i++) {
    if (pesos[i] < 40) {
      menosDe40++;
    } else if (pesos[i] >= 40 && pesos[i] < 50) {
      entre40y50++;
    } else if (pesos[i] >= 50 && pesos[i] < 60) {
      entre50y60++;
    } else if (pesos[i] >= 60) {
      masDe60++;
    }
  }

  // muestra de estadística
  console.log(`Alumnos con peso menor a 40 kg: ${menosDe40}`);
  console.log(`Alumnos con peso entre 40 kg y 50 kg: ${entre40y50}`);
  console.log(`Alumnos con peso entre 50 kg y 60 kg: ${entre50y60}`);
  console.log(`Alumnos con peso mayor o igual a 60 kg: ${masDe60}`);

document.getElementById("resp").innerHTML= respuesta;

}
