```mermaid
sequenceDiagram
    participant Usuario
    participant Navegador
    participant Servidor

    Usuario->>Navegador: Escribe una nueva nota y hace clic
    Navegador->>Servidor: POST /notes con contenido de la nota
    Servidor-->>Navegador: 200 OK + nota guardada
    Navegador-->>Usuario: Muestra la nueva nota en pantalla
