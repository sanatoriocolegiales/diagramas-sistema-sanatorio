flowchart TD
    A[Ingresos] --> B[Historia Clínica de Ingreso a Cirugía]
    B --> C[Intervencion]
    D[Epicrisis]
    C -->  E[Recuperacion]
    E --> H{Tipo Ingreso}
    H --> |Ambulatorio| D 
    H --> |Internado| I[UTI]
    H --> |Internado| J[UCO]
    H --> |Internado| K[Piso]
    D --> F[Egresos]
    I --> D
    J --> D
    K --> D
    I --> C
    J --> C
    K --> C
