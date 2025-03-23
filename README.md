# 0.6-Nueva-nota-
 Nueva nota en diagrama de aplicación de una sola pagina

  sequenceDiagram 

  participant Usuario

  participant Navegador

  participant Servidot

  Usuario->>Navegador: Escribe la nota y hace clic en "Guardar"

  Navegador->>Servidor: Post / new_note (con el contenido de la nueva nota)

  Servidor-->>Navegador: Responde con 201 created (nota creada)

  Navegador->>Navegador: Actualiza dinamicamente la vista de la pagina con la nueva nota
