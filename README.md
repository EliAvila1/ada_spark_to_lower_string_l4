# ada_spark_to_lower_string_l4

Una utilidad en **Ada / SPARK** completamente verificada formalmente (SPARK Nivel 4) para convertir cadenas de caracteres a minúsculas de forma segura.

## Especificaciones y Estado
El procedimiento está desarrollado bajo las directrices estrictas de SPARK para garantizar la ausencia de errores en tiempo de ejecución (Run-time Checks) y el cumplimiento de contratos funcionales.

```ada
procedure To_Lower_String with SPARK_Mode => On;
```

## Resumen del Análisis SPARK
reporte oficial generado por `gnatprove`. El proyecto cuenta con un **100% de éxito en la verificación**, resolviendo de manera automática todas las dependencias y aserciones.

```text
Summary of SPARK analysis
=========================

---------------------------------------------------------------------------------------------
SPARK Analysis results        Total       Flow   CodePeer      Provers   Justified   Unproved
---------------------------------------------------------------------------------------------
Data Dependencies                 1          1          .            .           .          .
Flow Dependencies                 1          1          .            .           .          .
Initialization                    1          1          .            .           .          .
Non-Aliasing                      .          .          .            .           .          .
Run-time Checks                  18          .          .    18 (CVC4)           .          .
Assertions                        6          .          .     6 (CVC4)           .          .
Functional Contracts              1          .          .     1 (CVC4)           .          .
LSP Verification                  .          .          .            .           .          .
Termination                       1          .          .     1 (CVC4)           .          .
Concurrency                       .          .          .            .           .          .
---------------------------------------------------------------------------------------------
Total                            29    3 (10%)          .     26 (90%)           .          .

Max steps used for successful proof: 1
Analyzed 1 unit
```

## Requisitos
* Compilador GNAT (Ada 2012 o superior)
* Herramientas de verificación SPARK (`gnatprove`)

in unit black_list_pswd, 1 subprograms and packages out of 1 analyzed
  black_list_pswd.To_Lower_Internal at black_list_pswd.adb:9 flow analyzed (0 errors, 0 checks and 0 warnings) and proved (26 checks)
  
