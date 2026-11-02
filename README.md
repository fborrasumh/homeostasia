# HomeostasIA

Laboratorio de Fisiología Animal: simula, razona y comprueba. Aplicación web de un solo fichero.

**Usar la app:** https://fborrasumh.github.io/homeostasia/

**Idiomas:** español (por defecto), inglés, portugués; selector en la barra superior (o `?lang=en` / `?lang=pt` en la URL).

## Qué hace

- **15 laboratorios** (3 + 3 + 2 + 2 + 2 + 3 por unidad) con simuladores calculados por código: termorregulación (bucle de retroalimentación por especie), potencial de membrana (Nernst, GHK) y potencial de acción (Hodgkin–Huxley), eje endocrino, gasto cardiaco con Frank–Starling y ECG, curva de la hemoglobina con efecto Bohr y altitud, ventilación alveolar, nefrón (Starling, umbral renal de la glucosa), equilibrio ácido-base (Henderson–Hasselbalch, Davenport), rumen (AGV, pH y metano por balance de hidrógeno), tubo digestivo comparado, ciclo estral, calendario de partos y espermatogénesis, curva de lactación de Wood, CCS del tanque y composición de la leche.
- Cada laboratorio tiene un **reto verificado por código** (los 15 se comprueban como alcanzables en las pruebas).
- **Test de control** (24 preguntas con explicación, repaso de fallos) y generador de **test imprimible en Word con clave**, con opciones barajadas de forma reproducible por semilla.
- **Seis casos clínicos** con datos, pistas locales y un tutor de IA opcional cuya respuesta se filtra por código si revela la solución.
- **Problemas individualizados por semilla** (8 plantillas) con solución calculada y diagnóstico de errores típicos (unidades, olvidar un factor, media simple en lugar de ponderada…).
- **Mapa mental** que se dibuja a partir del esquema del estudiante, con comprobación por código de los conceptos clave de la unidad.
- **Control de lectura** (la IA propone preguntas con cita literal; el código verifica que la cita está en el texto) y **juego de rol** con un ganadero simulado cuya lista de comprobación se verifica con la propia frase del estudiante.
- Glosario, informe de progreso en Word/CSV/JSON (copia de seguridad importable) y tres idiomas (español, inglés y portugués).
- Alineada con los componentes de evaluación del programa analítico (participación y mapas mentales, práctica, estudio de caso, roleplay y test de control).

## Cómo se usa la IA

La IA es **opcional** (tutor de casos, preguntas sobre el esquema, control de lectura y juego de rol). Con la propia clave de OpenAI, Google Gemini o Anthropic Claude. La clave se guarda solo en el navegador. No hace falta servidor.

## Privacidad

Todo se calcula y se guarda en el navegador (IndexedDB). Solo si el usuario usa la IA, el texto que escribe (pregunta al tutor, esquema, pasaje de lectura, preguntas del rol) sale hacia su proveedor con correo, teléfono, DNI/NIE y similares enmascarados, y **antes del primer envío de la sesión se muestra una muestra de lo que sale** y se pide confirmación. La clave de IA la pone cada persona y no figura en el código.

## Límites

- Los modelos son **didácticos**: reproducen el comportamiento cualitativo y órdenes de magnitud de manual; no sustituyen a la clínica ni a la medición. Los valores por especie (frecuencias, umbrales, composición de la leche, duraciones de ciclo y gestación) son **orientativos**: contrástalos con Cunningham o Moyes antes de usarlos en un examen.
- El modelo de Hodgkin–Huxley es el del axón gigante de calamar a 6,3 °C: ilustra el principio, no un axón de mamífero.
- Los temas 1–4 se han asignado a la unidad I y los 5–8 a la II (el programa analítico no los separa por unidad); el sistema nervioso y el endocrino, citados en el título de la unidad I, se trabajan en dos laboratorios.
- Nunca se probó con una clave real de IA: las pruebas usan respuestas simuladas (incluidas una cita inventada y una frase del tutor que revela la solución, que el código detecta). El filtro del tutor es heurístico y no garantiza que no se filtre una pista.
- La IA puede equivocarse; la decisión y la evaluación final son siempre del profesorado y del estudiante.

## Autoría

Fernando Borrás Rocher (Universidad Miguel Hernández de Elche) y Hernán Rigoberto Benavides Rosales (Universidad Politécnica Estatal del Carchi (UPEC), Tulcán, Ecuador).

A partir del programa analítico de Fisiología Animal (código 0811BFA5UB-AJ2025, Carrera de Agropecuaria, Facultad de Industrias Agropecuarias y Ciencias Ambientales, UPEC, Tulcán) elaborado por el docente Hernán Rigoberto Benavides Rosales.

ORCID: Fernando Borrás Rocher [0000-0002-5519-4573](https://orcid.org/0000-0002-5519-4573) · Hernán Rigoberto Benavides Rosales [0009-0005-4934-6533](https://orcid.org/0009-0005-4934-6533)

## Cómo citar

Borrás Rocher, F. y Benavides Rosales, H. (2026). *HomeostasIA* (v1.0.0) [Software]. (DOI en trámite)

## Licencia

MIT. Véase [LICENSE](LICENSE).
