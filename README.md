# Proyecto MiSE — Custom PCB

View this project on [CADLAB.io](https://cadlab.io/project/30101).

PCB diseñada para la asignatura de Microcontroladores i Sistemes Empotrats (MiSE) de la Universitat de Barcelona. El diseño fue realizado íntegramente en KiCad, incluyendo esquemático, layout y exportación de Gerbers.

## Hardware

| Componente | Descripción |
|---|---|
| MSP430FR2355TPT | Microcontrolador TI MSP430, 48-pin QFP, bajo consumo |
| LMV324 | Amplificador operacional cuádruple (acondicionamiento de señal) |
| THB001P | Switch codificador (C&K Components, 14 pines) |
| LCD 2×16 I2C | Display alfanumérico con interfaz I2C (Midas) |
| LDR | Fotorresistencia para detección de luz |
| WIFI | Módulo de conectividad inalámbrica |
| Crystal | Oscilador de cristal externo |
| Pasivos SMD | Resistencias y condensadores en encapsulado 0805 |

## Estructura del repositorio
├── PCB_MiSE.kicad_pcb       # Layout de la PCB
├── PCB_MiSE.kicad_sch       # Esquemático
├── PCB_MiSE.kicad_pro       # Archivo de proyecto KiCad
├── Gerbers/                  # Archivos de fabricación
├── Componentes/
│   └── MiSE.pretty/         # Librería de footprints personalizada
└── PCB_MiSE-backups/        # Backups automáticos de KiCad

## Fabricación

Los archivos Gerber listos para enviar a fabricar están en la carpeta `Gerbers/`. El diseño es una PCB de 2 capas con componentes SMD (0805) y through-hole.

## Herramientas

- [KiCad](https://www.kicad.org/) 8.x
- [CADLAB.io](https://cadlab.io) — revisión visual de cambios en el PCB