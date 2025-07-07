# Vamos a la ruta de trabajo y usamos un dckerfile multietapa
WORKDIR /app

# Copia el binario al contenedor
COPY binario /app

# Define el comando a ejecutar al iniciar el contenedor
CMD ["./binario"]

#Ejecutamos el binario
RUN  --from=builder /root/.local /home/${APP_USER}/.local

    



