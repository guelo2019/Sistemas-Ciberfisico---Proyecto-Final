
![CIP](https://github.com/guelo2019/Sistemas-Ciberfisico---Proyecto-Final/assets/46485082/ad69c717-6e3b-4a77-9b69-1b2c7fae009b)

# 1) **Sistema CIP:** 

### Clean In Place (Limpieza en el lugar) CIP (Clean-In-Place):

Es un método utilizado para limpiar las tuberías, tanques, actuadores y otros equipos utilizados en procesos, especialmente en la industria alimentaria, sin desmontarlos. Un sistema CIP utiliza fluidos de 
limpieza (como soluciones de soda cáustica) y agua para eliminar la suciedad, los residuos de alimentos y otros contaminantes de las superficies del equipo. Esta limpieza suele seguirse de un enjuague con agua caliente y finalmente con agua fría para asegurar que no 
queden residuos químicos en el equipo. Diseño de Lógica de Control para el Proceso de CIP con Tres Tanques

## 2) **Objetivo:** 
Modificar el esquema del ejercicio 1 y desarrollar una lógica de control que automatice el proceso de limpieza CIP con tres tanques: soda cáustica, agua caliente y agua fría. 

### **Componentes:**

- [x] Pilotos LED: H1, H2, H3 
- [x] Pulsadores: Rt, PG, PM 
- [x] Bombas: M1 (carga), M2 (envío) 
- [x] Válvulas: V1 (entrada de soda cáustica), V2 (entrada de agua caliente), V3 (entrada de agua fría), V4 (salida/vaciado general) 
- [x] Sensores de Nivel: B2 (nivel mínimo), B1 (nivel máximo) 

# Tareas:

>## Fase de Soda Cáustica:
- [x] Al presionar PM, M1 se activa y V1 se abre para llenar el tanque de soda cáustica. 
- [x] H1 se enciende en verde mientras el tanque se está llenando con soda cáustica. 
- [x] Una vez alcanzado el nivel deseado, V1 se cierra. 

>## Fase de Agua Caliente:

- [x] Con M1 aún en funcionamiento, V2 se abre para llenar el tanque de agua caliente. 
- [x] H2 se enciende en verde mientras el tanque se está llenando con agua caliente. 
- [x] Tras alcanzar el nivel deseado, V2 se cierra. 

>## Fase de Agua Fría:

- [x] M1 sigue funcionando y V3 se abre para llenar el tanque con agua fría. 
- [x] H1 y H2 se apagan, y H3 se enciende en verde durante esta fase. 
- [x] Una vez alcanzado el nivel deseado, V3 se cierra. 

>## Selección del Tanque para CIP:

- [x] Luego de la preparación, se activará la bomba M2 que seleccionará el tanque adecuado para comenzar con el proceso CIP en la maquinaria y procesos correspondientes. 

>## Vaciado y Finalización:

- [x] V4 se abrirá para vaciar completamente los tanques si es necesario. 
- [x] Una vez vaciado, todos los pilotos se apagan indicando la finalización del proceso.

**PG :** es una parada de emergencia. Al presionarse, todo el proceso debe detenerse inmediatamente. H3 se encenderá en rojo cuando se active la parada de emergencia. 

**Rt :** sirve para reiniciar el proceso en caso de que se haya detenido por alguna alarma o interrupción. 

# Tarea:

Diseñe la lógica de control adaptando el esquema anterior a este nuevo proceso. Puede usar lógica cableada, Ladder, Funcional o Grafcet. Asegúrese de considerar todas las fases y proporcionar una solución robusta y segura. 
