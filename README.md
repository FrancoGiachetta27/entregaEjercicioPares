# Ejercicio Cuidandonos

Integrantes:
- Franco Giachetta
- Agustin Gonzalez Canosa

## Solución punto 1)
![image](https://github.com/FrancoGiachetta27/entregaEjercicioPares/assets/83255667/8f35cfb7-257d-4478-94c8-59cdd6f133b5)

## Solución punto 2)
![image](https://github.com/FrancoGiachetta27/entregaEjercicioPares/assets/83255667/df759f7b-a4ec-4a4b-90f2-146d4525d0fc)


## Pseudocódigo
```java
class Vieje {
  destino: List<Destino>
...
  public Integer calcularTiempoAproximadoViaje() {
      Integer tiempoViajeAprox = 0;
      CalculadoraTiempoViaje calculadora = new CalculadoraTiempoViaje();
      for(Integer i=0; i<destino.length-1; i++) {
          tiempoViajeAprox += calculadora.calcularTiempoViaje(destino[i].ubicacion, destino[i+1].ubicacion) + destino[i+1].tiempoEspera;
      }
      return tiempoViajeAprox;
  }
}
```
