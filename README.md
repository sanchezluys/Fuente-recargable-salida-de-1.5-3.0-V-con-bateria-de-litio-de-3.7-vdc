# Fuente-recargable-salida-de-1.5-3.0-V-con-bateria-de-litio-de-3.7-vdc

```mermaid
graph TD
    subgraph Módulo de Carga USB-C TP4056
        A[Puerto USB-C] --> B{Circuito de Carga TP4056}
        B -- Conexión a Batería --> C[Terminales B+ y B-]
    end

    subgraph Módulo Reductor Buck Converter
        E[Terminales IN+ y IN-] -- Conexión de Entrada --> F{Circuito Reductor}
        F -- Salida Regulada --> G[Terminales OUT+ y OUT-]
    end

    H[Batería de Litio 3.7V] -- Conectar a --> C
    C -- Conectar a --> E
    G -- Conectar a --> I[Equipo a alimentar 3V / 1.5V y GND]

    style H fill:#f9f,stroke:#333,stroke-width:2px
    style I fill:#ccf,stroke:#333,stroke-width:2px
```
