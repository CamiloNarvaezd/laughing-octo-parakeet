distacia, velocidad_max, tiempo= input().split()
distacia = float(distacia)
velocidad_max = float(velocidad_max)
tiempo = float(tiempo)

velocidad_resultado = (distacia / 1000) / (tiempo/3600)

if (distacia < 0 or velocidad_max < 0 or tiempo < 0):
        print("ERROR")
elif (velocidad_resultado <= velocidad_max):
    print("VELOCIDAD NORMAL")
elif (velocidad_resultado > velocidad_max and velocidad_resultado < velocidad_max * 1.2):
    print("NUEVO RECORD") 
else:
    print("ENTREVISTA")
