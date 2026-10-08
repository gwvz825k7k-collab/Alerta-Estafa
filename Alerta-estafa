import streamlit as st

st.title("Alerta Estafa")
st.subheader("Ciberestafas")

# Filas: 0 = Premio falso | 1 = Enlace sospechoso | 2 = Falso familiar
# Columnas: 0 = Nombre del riesgo | 1 = Señal de alerta | 2 = Acción preventiva

matriz_ciber = [
    ["Premio falso",
     "Dicen que ganaste un premio y piden tus datos mediante un enlace.",
     "No des tus datos ni entres al enlace."],

    ["Enlace sospechoso",
     "Dicen que tu cuenta será bloqueada y envían un enlace.",
     "No abras el enlace y revisa tu cuenta desde la aplicación oficial."],

    ["Falso familiar",
     "Alguien se hace pasar por un familiar y pide dinero urgentemente.",
     "Llama al familiar para confirmar antes de enviar dinero."]
]

st.info("Selecciona un riesgo para consultar la base de datos.")

opcion_riesgo = st.selectbox(
    "1. Selecciona el riesgo:",
    ["Ciberestafa: premio falso",
     "Ciberestafa: enlace sospechoso",
     "Ciberestafa: falso familiar"]
)

if opcion_riesgo == "Ciberestafa: premio falso":
    fila = 0
elif opcion_riesgo == "Ciberestafa: enlace sospechoso":
    fila = 1
else:
    fila = 2

opcion_dato = st.radio(
    "¿Qué información necesitas?",
    ["Nombre del riesgo", "Señal de alerta", "Acción preventiva"]
)

if opcion_dato == "Nombre del riesgo":
    columna = 0
elif opcion_dato == "Señal de alerta":
    columna = 1
else:
    columna = 2

if st.button("Consultar matriz de datos"):
    resultado = matriz_ciber[fila][columna]
    st.success(f"Resultado: {resultado}")
    
