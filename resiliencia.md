Mesa redonda sobre resiliencia
==============================

Questions
---------

  1. Qué es la resiliencia de sistemas para ti?

  Básicamente que el **negocio pueda seguir operando ante circustancias anómalas**, y/o que la **degradación sea controlada**.
  **Nivel de resistencia a los estresores** Behavior changes continuously. Impermanencia. Consistencia del negocio (consistencia de datos y procesos).


  2. A nivel técnico y personal que es un must a tener cuando hablamos de sistemas resilientes? Autoescalabilidad, auto healing, monitoring, alerting, etc...

  **Monitorización y alertas**. Auditoría. Trazar acciones de usuarios. **Redundancia**. **Reducción de los SPoF** (Single Points of Failure) de sistemas (internos y externos) **y de proveedores**. **Fail-fast** (*fail-fast is not test and fail*). Procesos de **continous delivery/deployment**. PasS. Infraestructura manejada.

Automatización. Toggle feature. Circuit breaker. . Intentar reducir incepridumbre en *la zona desconocida* (unk-unk area). Sitios donde no controlas las entradas.

Caso de los DNSs, Twitter, Whatsapp images y el porno. 
    

  3. Cómo transformas una empresa "old school"? Cuáles son las trabas más grandes que te puedes encontrar?

  Básicamente **Agile**, cultura **DevOps** y **Arquitectura**. Mecanización y automatización de tareas.
  
  Las trabas básicamente han sido **humanas**. Reticencia al **cambio**. Costes.


  4. Has tenido algún momento en el que has dicho: gracias a $DEITY que hemos invertido en implantar esto.

  No exactamente, pero cuando petó todo por culpa de un **certificado de un firewall** (anécdota) y nos fuimos a tomar una cerveza sirvio a z+ para confirmar que estábamos en el camino correcto.


---

  Aplicaciones--> robustos
  Sistemas --> resilientes
  Organizaciones --> antifrágiles  (Estudiar si esto es correcto al 100%)

Automatizar para reducir human factor (caso de la revocación de certificado de firewall de z+)

Third party providers: el caso del DDoS a servidores DNS y la caída de Twitter, etc. El porno (youporn no cayo)

Cultura DevOps


When they say "x does not scale", they doesn't mean x-made systems cannot be large. Just that the cost increase is not linear.

Fail-fast is not test and error


---

Documento de ideas
------------------

  - Contar de algún caso que conozcamos o que nos haya pasado, relacionado con estos temas (caidas de sistemas, como afectaron, qué medidas se tomaron, ...).
  - Yo (javier) creo que la resiliencia es un tema en el que importa tanto -o más- la parte cultural/soft skills como la parte técnica. Una cosa que me interesa es cómo implementar una cultura de fiabilidad (llamálo SRE o incluso devops si prefieres) en tu entorno.
  - También me parece interesante ver cómo la gente empieza a hacer SRE, qué procedimientos/scripts/herramientas implementaste al principio y tuvieron impacto en tu fiabilidad. Creo que de cara a la parte divulgativa viene bien porque puede dar ideas a gente que todavía no tenga nada, pero que quiera empezar con algo simple y con cierto impacto (igual tan fácil como usar monit para rearrancar procesos, o añadir un health check para tirar un contenedor/instancia y añadir otro al LB cuando no responde).
  - Y junto a esto, lo contrario.. Preguntar a la gente lo más sofisticado que tienen en su política de fiabilidad, que yo creo que siempre gusta contar lo bien que haces las cosas.
  - Y para bajar al mundo real, lo mismo preguntando por qué no tienen una cultura de fiabilidad ahora mismo en sus empresas tenemos participación. A la gente le gusta contar lo malos que son sus jefes y los problemas que se están encontrando para poder hacer las cosas bien.

