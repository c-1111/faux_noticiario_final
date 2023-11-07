<template>
    <div id="1"
        class="noticia border-l-1 border-r-1 border-t-0 border-black border max-[800px]:max-w-[800px] max-[800px]:border-r-0 max-[800px]:border-b-1 max-[800px]:border-l-0"
        v-show="isHidden">
        <div class="noticia_holder">
            <div class="noticia_top">
                <div class="titular sty_titular">Tragedia en el Corazón de la Ciudad: Atentado Terrorista Deja un Rastro de
                    Muerte y Dolor</div>
                <div class="subtitulo sty_subtitulo">Explosión Devasta el Centro de la Ciudad de México, la acción es atribuida al grupo terrorista XIA</div>
                <div class="top_info">
                    <div class="lugar sty_lugar">Ciudad de México, México</div>
                    <div class="timeago sty_tiempo ">hace 2 horas</div>
                </div>
            </div>
            <div
                class="noticia_bottom flex flex-row w-full justify-between gap-12 pt-2 pb-0 max-[800px]:grid max-[800px]:grid-cols-1 max-[800px]:pt-2">
                <div class="noticia_btm_left">
                    <div class="autor max-w-[50ch] font-lora font-light text-[15px] text-zinc-800 max-[800px]:text-[14px]">
                        Un devastador atentado terrorista sacudió el centro de la ciudad en un día que quedará marcado por
                        la tragedia. Al menos 20 personas perdieron la vida y otras 50 resultaron heridas en un acto de
                        violencia que conmocionó a la población. El ataque se llevó a cabo en una concurrida plaza durante
                        el horario de mayor afluencia de personas, cuando un vehículo cargado de explosivos estalló frente a
                        un edificio gubernamental.

                        El caos y el horror se apoderaron del lugar, mientras los servicios de emergencia se apresuraban a
                        atender a los heridos y a trasladarlos a hospitales cercanos. La magnitud de la explosión dejó
                        edificios cercanos gravemente dañados, y el equipo de rescate trabaja incansablemente en busca de
                        posibles sobrevivientes entre los escombros.

                        Las autoridades han desplegado un importante operativo de seguridad en la zona y han iniciado una
                        exhaustiva investigación para determinar la autoría y los motivos detrás de este atentado brutal. Se
                        han implementado medidas adicionales de seguridad en toda la ciudad, y se insta a la población a
                        mantener la calma y colaborar con cualquier información relevante que pueda ayudar en la
                        investigación.

                        Las muestras de solidaridad y apoyo de la comunidad no se hicieron esperar, con personas y
                        organizaciones ofreciendo ayuda a las víctimas y a sus familias en este momento de dolor y angustia.
                        La ciudad se une en su rechazo a la violencia y en su determinación de superar esta tragedia juntos.

                    </div>
                    <div class="autor font-sf font-light text-[13px] pt-4 text-zinc-400 animate-pulse max-[800px]:pt-10">
                        Noticia generada por {{ inputValue }} </div>
                </div>
                <div class="noticia_btm_right max-h-[500px] max-[800px]:max-w-[800px] max-[800px]:justify-items-center">
                    <img src="/noticias/atentado.jpg" alt="imagen de la noticia" class=" max-h-[500px] max-[800px]:max-w-[325px]">
                </div>

            </div>
        </div>
    </div>

    <div id="2"
        class="noticia border-l-1 border-r-1 border-t-0 border-black border max-[800px]:max-w-[800px] max-[800px]:border-r-0 max-[800px]:border-b-1 max-[800px]:border-l-0">
        <div class="noticia_holder">
            <div class="noticia_top">
                <div class="titular sty_titular">"Innovación en el Tablero: El Comité de Ajedrez Anuncia una Nueva Pieza"
                </div>
                <div class="subtitulo sty_subtitulo">"El ajedrez se reinventa con la introducción de 'El Dragón' en su
                    repertorio de piezas"</div>
                <div class="top_info">
                    <div class="lugar sty_lugar">Lausitz, Alemania</div>
                    <div class="timeago sty_tiempo ">hace 17 horas</div>
                </div>
            </div>
            <div
                class="noticia_bottom flex flex-row w-full justify-between gap-12 pt-2 pb-0 max-[800px]:grid max-[800px]:grid-cols-1 max-[800px]:pt-2">
                <div class="noticia_btm_left">
                    <div class="autor max-w-[50ch] font-lora font-light text-[15px] text-zinc-800 max-[800px]:text-[14px]">
                        En un emocionante giro de los acontecimientos, la Federación Internacional de Ajedrez ha anunciado
                        oficialmente la introducción de una nueva pieza en el juego milenario. Conocida como "El Dragón",
                        esta pieza promete revolucionar la estrategia y la dinámica del ajedrez como lo conocemos.

                        El comité, compuesto por los principales maestros del ajedrez y expertos en la materia, ha trabajado
                        en secreto durante años para desarrollar esta pieza innovadora. "El Dragón" se mueve en forma de L,
                        similar al caballo, pero con un giro único. Su introducción se realiza con el objetivo de inyectar
                        nueva vida en el juego y desafiar a los ajedrecistas a repensar sus estrategias.

                        El presidente de la Federación Internacional de Ajedrez, el ficticio Dr. Anton Fischer, declaró:
                        "Estamos emocionados de presentar 'El Dragón' al mundo del ajedrez. Esta nueva pieza agregará un
                        elemento de sorpresa y creatividad al juego, y esperamos que los jugadores de todos los niveles
                        disfruten de su inclusión".

                        Los ajedrecistas de todo el mundo están ansiosos por poner a prueba esta nueva pieza en sus
                        partidas, y los torneos de ajedrez ya han comenzado a adaptar sus reglas para acomodar "El Dragón".
                        Se espera que esta innovación despierte un renovado interés en el ajedrez y que los jugadores
                        exploren estrategias completamente nuevas.

                        Aunque algunos puristas del ajedrez han expresado preocupaciones sobre la alteración de las reglas
                        tradicionales, la Federación Internacional de Ajedrez confía en que esta adición impulsará el juego
                        hacia el futuro.</div>
                    <div class="autor font-sf font-light text-[13px] pt-4 text-zinc-400 animate-pulse max-[800px]:pt-10">
                        Escrita por Markus Schneider, Corresponsal de Ajedrez </div>
                </div>
                <div class="noticia_btm_right max-h-[500px] max-[800px]:max-w-[800px] max-[800px]:justify-items-center">
                    <img src="/noticias/comite_ajedrez.jpg" alt="imagen de la noticia"
                        class=" max-h-[500px] max-[800px]:max-w-[325px]">
                </div>

            </div>
        </div>
    </div>

    <div id="3"
        class="noticia border-l-1 border-r-1 border-t-0 border-black border max-[800px]:max-w-[800px] max-[800px]:border-r-0 max-[800px]:border-b-1 max-[800px]:border-l-0">
        <div class="noticia_holder">
            <div class="noticia_top">
                <div class="titular sty_titular">Preocupación por Injerencias Extranjeras en las Elecciones Francesas</div>
                <div class="subtitulo sty_subtitulo">Las autoridades francesas investigan posibles intentos de influencia
                    extranjera en el proceso electoral</div>
                <div class="top_info">
                    <div class="lugar sty_lugar">París, Francia</div>
                    <div class="timeago sty_tiempo ">hace 3 días</div>
                </div>
            </div>
            <div
                class="noticia_bottom flex flex-row w-full justify-between gap-12 pt-2 pb-0 max-[800px]:grid max-[800px]:grid-cols-1 max-[800px]:pt-2">
                <div class="noticia_btm_left">
                    <div class="autor max-w-[50ch] font-lora font-light text-[15px] text-zinc-800 max-[800px]:text-[14px]">A
                        medida que Francia se prepara para las próximas elecciones, las alarmas han sonado debido a las
                        crecientes preocupaciones sobre posibles injerencias extranjeras en el proceso democrático. Las
                        autoridades francesas están tomando medidas para investigar y abordar cualquier interferencia en la
                        elección.

                        Las agencias de seguridad y los expertos en ciberseguridad han detectado actividades sospechosas en
                        línea, incluyendo intentos de desinformación y ataques cibernéticos dirigidos a actores políticos.
                        Aunque aún no se han identificado a los responsables, se cree que estos intentos provienen de
                        actores extranjeros que buscan influir en los resultados de las elecciones.

                        El presidente ficticio de Francia, Jean Dupont, emitió una declaración en la que expresó su
                        preocupación por estas actividades. "La integridad de nuestras elecciones es fundamental para
                        nuestra democracia. No permitiremos que actores extranjeros socaven la voluntad del pueblo francés",
                        declaró Dupont.

                        Las agencias de inteligencia francesas y las fuerzas de seguridad cibernética están trabajando en
                        estrecha colaboración para rastrear y contrarrestar estas amenazas. Se han intensificado los
                        esfuerzos para educar al público sobre la desinformación y la ciberseguridad, y se han implementado
                        medidas adicionales de seguridad en el proceso electoral.

                        El Ministro de Asuntos Exteriores, Marie Leclerc, ha llamado a la comunidad internacional a condenar
                        cualquier intento de interferencia en las elecciones francesas y a respetar la soberanía de Francia
                        en asuntos electorales.
                    </div>
                    <div class="autor font-sf font-light text-[13px] pt-4 text-zinc-400 animate-pulse max-[800px]:pt-10">
                        Escrita por Pierre Dubois, Corresponsal de Política Internacional </div>
                </div>
                <div class="noticia_btm_right  max-[800px]:max-w-[800px] max-[800px]:justify-items-center">
                    <img src="/noticias/francia2.jpg" alt="imagen de la noticia"
                        class=" max-h-[500px] max-[800px]:max-w-[325px]">
                </div>

            </div>
        </div>
    </div>

    <div id="4"
        class="noticia border-l-1 border-r-1 border-t-0 border-black border max-[800px]:max-w-[800px] max-[800px]:border-r-0 max-[800px]:border-b-1 max-[800px]:border-l-0">
        <div class="noticia_holder">
            <div class="noticia_top">
                <div class="titular sty_titular">Aumento de los Encuentros Inusuales: Orcas Desencadenan Auge en la Venta de
                    Armas en las Costas de España</div>
                <div class="subtitulo sty_subtitulo">Un Dilema entre Fauna y Seguridad: Orcas Desatan la Incertidumbre en
                    las Costas Españolas</div>
                <div class="top_info">
                    <div class="lugar sty_lugar">Costa Española</div>
                    <div class="timeago sty_tiempo ">hace 7 días</div>
                </div>
            </div>
            <div
                class="noticia_bottom flex flex-row w-full justify-between gap-12 pt-2 pb-0 max-[800px]:grid max-[800px]:grid-cols-1 max-[800px]:pt-2">
                <div class="noticia_btm_left">
                    <div class="autor max-w-[50ch] font-lora font-light text-[15px] text-zinc-800 max-[800px]:text-[14px]">
                        En las costas de España, un fenómeno sorprendente ha estado en aumento: los encuentros inusuales con
                        orcas han llevado a un auge en la venta de armas entre pescadores y empresas turísticas. Estos
                        incidentes, que han incluido daños en barcos y heridas a los tripulantes, han generado temor entre
                        los residentes locales y visitantes, quienes buscan soluciones para proteger sus embarcaciones y su
                        seguridad.

                        Las orcas, conocidas por su inteligencia y agilidad, han estado protagonizando encuentros cada vez
                        más frecuentes en las aguas costeras de España. Si bien estos animales marinos son generalmente
                        pacíficos, algunos incidentes han generado preocupación, especialmente entre aquellos que dependen
                        de la pesca y el turismo.

                        A pesar de las recomendaciones de las autoridades y expertos en conservación marina para adoptar
                        medidas no letales, como el uso de sonidos de alta frecuencia o redes de protección, muchos
                        pescadores y empresas turísticas han optado por la compra de armas de fuego para disuadir a los
                        animales. Esta tendencia ha planteado un debate complejo sobre el equilibrio entre la protección de
                        la fauna marina y la seguridad humana en la costa española.

                        Los expertos en conservación marina han expresado su preocupación por la respuesta de algunos
                        individuos, señalando que las armas de fuego no son una solución sostenible y plantean riesgos
                        adicionales para la vida marina y el entorno marino. Instan a la implementación de medidas no
                        letales que permitan coexistir de manera segura con estas criaturas impresionantes.

                        El aumento de los encuentros inusuales con orcas en las costas de España ha abierto un diálogo
                        importante sobre cómo equilibrar la protección de la fauna marina con la seguridad de las personas,
                        y se espera que las autoridades y la comunidad local trabajen juntas para abordar este desafío en
                        evolución.
                    </div>
                    <div class="autor font-sf font-light text-[13px] pt-4 text-zinc-400 animate-pulse max-[800px]:pt-10">
                        Escrita por María Marítima </div>
                </div>
                <div class="noticia_btm_right max-h-[500px] max-[800px]:max-w-[800px] max-[800px]:justify-items-center">
                    <img src="/noticias/orcas2.jpg" alt="imagen de la noticia"
                        class=" max-h-[500px] max-[800px]:max-w-[325px]">
                </div>

            </div>
        </div>
    </div>

    <div id="5"
        class="noticia border-l-1 border-r-1 border-t-0 border-black border max-[800px]:max-w-[800px] max-[800px]:border-r-0 max-[800px]:border-b-1 max-[800px]:border-l-0">
        <div class="noticia_holder">
            <div class="noticia_top">
                <div class="titular sty_titular">Preocupante Descubrimiento: Declive en el Coeficiente Intelectual de los
                    Niños del Siglo XXI</div>
                <div class="subtitulo sty_subtitulo">El Impacto de la Tecnología, la Falta de Interacción Social y la
                    Educación en la Inteligencia de los Niños Modernos</div>
                <div class="top_info">
                    <div class="lugar sty_lugar">Investigación Internacional</div>
                    <div class="timeago sty_tiempo ">hace 1 semana</div>
                </div>
            </div>
            <div
                class="noticia_bottom flex flex-row w-full justify-between gap-12 pt-2 pb-0 max-[800px]:grid max-[800px]:grid-cols-1 max-[800px]:pt-2">
                <div class="noticia_btm_left">
                    <div class="autor max-w-[50ch] font-lora font-light text-[15px] text-zinc-800 max-[800px]:text-[14px]">
                        En un sorprendente hallazgo, un estudio reciente ha revelado que los niños de la actualidad poseen
                        un coeficiente intelectual más bajo en comparación con generaciones pasadas. Este declive en la
                        inteligencia infantil ha encendido alarmas entre educadores y expertos en el desarrollo infantil,
                        quienes apuntan a varios factores que podrían estar contribuyendo a esta tendencia preocupante.

                        Los investigadores han identificado una serie de razones detrás de este descenso en el coeficiente
                        intelectual de los niños. Uno de los principales factores es la exposición excesiva a la tecnología
                        desde una edad temprana. El constante acceso a dispositivos electrónicos y pantallas ha llevado a
                        una disminución en las habilidades cognitivas y de resolución de problemas, a medida que los niños
                        pasan más tiempo consumiendo contenido en línea en lugar de participar en actividades estimulantes.

                        La falta de interacción social cara a cara también ha demostrado ser un factor influyente. El
                        aislamiento social, a menudo impulsado por la tecnología, ha reducido las oportunidades de los niños
                        para desarrollar habilidades sociales, empatía y comunicación efectiva. Esta carencia de interacción
                        interpersonal puede tener efectos a largo plazo en su desarrollo intelectual y emocional.

                        Además, los expertos señalan el deterioro de la calidad educativa como un tercer factor clave. La
                        presión sobre el sistema educativo, la falta de recursos y la sobrecarga de los educadores pueden
                        resultar en una educación menos efectiva. Esto afecta la capacidad de los niños para adquirir
                        conocimientos y desarrollar habilidades intelectuales de manera óptima.
                    </div>
                    <div class="autor font-sf font-light text-[13px] pt-4 text-zinc-400 animate-pulse max-[800px]:pt-10">
                        Escrita por Juan Garrido </div>
                </div>
                <div class="noticia_btm_right max-h-[500px] max-[800px]:max-w-[800px] max-[800px]:justify-items-center">
                    <img src="/noticias/nenos.jpg" alt="imagen de la noticia"
                        class=" max-h-[500px] max-[800px]:max-w-[325px]">
                </div>

            </div>
        </div>
    </div>

    <div id="6"
        class="noticia border-l-1 border-r-1 border-t-0 border-black border max-[800px]:max-w-[800px] max-[800px]:border-r-0 max-[800px]:border-b-1 max-[800px]:border-l-0">
        <div class="noticia_holder">
            <div class="noticia_top">
                <div class="titular sty_titular">Controversia en Barcelona: Nuevo Vertedero Nuclear en el Corazón de la
                    Ciudad Despierta la Ira de Residentes</div>
                <div class="subtitulo sty_subtitulo">La Batalla entre Seguridad y Medio Ambiente: La Polémica Construcción
                    del Vertedero Nuclear en Barcelona</div>
                <div class="top_info">
                    <div class="lugar sty_lugar">Barcelona, España</div>
                    <div class="timeago sty_tiempo ">hace 2 semana</div>
                </div>
            </div>
            <div
                class="noticia_bottom flex flex-row w-full justify-between gap-12 pt-2 pb-0 max-[800px]:grid max-[800px]:grid-cols-1 max-[800px]:pt-2">
                <div class="noticia_btm_left">
                    <div class="autor max-w-[50ch] font-lora font-light text-[15px] text-zinc-800 max-[800px]:text-[14px]">
                        Una tormenta de controversia ha envuelto a Barcelona después de que se anunciara la construcción de
                        un nuevo vertedero nuclear en pleno centro de la ciudad. El proyecto ha desatado una ola de críticas
                        por parte de los residentes y grupos ecologistas, quienes expresan profundas preocupaciones sobre
                        los riesgos que implica albergar residuos radiactivos en una ubicación tan cercana a la población.

                        Los promotores del proyecto argumentan que el terreno ha sido seleccionado meticulosamente y que se
                        han implementado rigurosas medidas de seguridad para salvaguardar el medio ambiente y la salud
                        pública. Afirman que el vertedero nuclear es necesario para gestionar adecuadamente los residuos
                        radiactivos generados en la región y que su construcción cumple con las regulaciones más estrictas.

                        Sin embargo, los opositores al proyecto insisten en la necesidad de explorar alternativas menos
                        arriesgadas. Temen las posibles consecuencias a largo plazo de albergar material radiactivo en una
                        ubicación tan densamente poblada, argumentando que incluso con medidas de seguridad, el riesgo
                        siempre está presente.

                        La controversia ha llevado a manifestaciones y debates en la ciudad, donde los residentes expresan
                        su temor por la seguridad y el impacto en la calidad de vida. Además, grupos ecologistas han
                        intensificado sus esfuerzos para concienciar sobre los riesgos ambientales que conlleva la
                        construcción del vertedero nuclear en el centro de Barcelona.

                        El dilema entre seguridad y medio ambiente ha dejado a la ciudad dividida y a las autoridades en un
                        aprieto. Mientras se intensifican las discusiones, se espera que se realicen evaluaciones
                        exhaustivas y que se incluyan todas las voces en la toma de decisiones sobre este controvertido
                        proyecto. La construcción del vertedero nuclear en el corazón de Barcelona continúa siendo un tema
                        candente de debate en la ciudad
                    </div>
                    <div class="autor font-sf font-light text-[13px] pt-4 text-zinc-400 animate-pulse max-[800px]:pt-10">
                        Escrita por Julia Díaz </div>
                </div>
                <div class="noticia_btm_right max-h-[500px] max-[800px]:max-w-[800px] max-[800px]:justify-items-center">
                    <img src="/noticias/bcn1.jpg" alt="imagen de la noticia"
                        class=" max-h-[500px] max-[800px]:max-w-[325px]">
                </div>

            </div>
        </div>
    </div>

    <!-- <div id="7"
        class="noticia border-l-1 border-r-1 border-t-0 border-black border max-[800px]:max-w-[800px] max-[800px]:border-r-0 max-[800px]:border-b-1 max-[800px]:border-l-0">
        <div class="noticia_holder">
            <div class="noticia_top">
                <div class="titular sty_titular"></div>
                <div class="subtitulo sty_subtitulo"></div>
                <div class="top_info">
                    <div class="lugar sty_lugar"></div>
                    <div class="timeago sty_tiempo "></div>
                </div>
            </div>
            <div
                class="noticia_bottom flex flex-row w-full justify-between gap-12 pt-2 pb-0 max-[800px]:grid max-[800px]:grid-cols-1 max-[800px]:pt-2">
                <div class="noticia_btm_left">
                    <div class="autor max-w-[50ch] font-lora font-light text-[15px] text-zinc-800 max-[800px]:text-[14px]">
                    </div>
                    <div class="autor font-sf font-light text-[13px] pt-4 text-zinc-400 animate-pulse max-[800px]:pt-10">
                        Escrita por Miguel Gómez </div>
                </div>
                <div class="noticia_btm_right max-h-[500px] max-[800px]:max-w-[800px] max-[800px]:justify-items-center">
                    <img src="" alt="imagen de la noticia" class=" max-h-[500px] max-[800px]:max-w-[325px]">
                </div>

            </div>
        </div>
    </div>

    <div id="8"
        class="noticia border-l-1 border-r-1 border-t-0 border-black border max-[800px]:max-w-[800px] max-[800px]:border-r-0 max-[800px]:border-b-1 max-[800px]:border-l-0">
        <div class="noticia_holder">
            <div class="noticia_top">
                <div class="titular sty_titular"></div>
                <div class="subtitulo sty_subtitulo"></div>
                <div class="top_info">
                    <div class="lugar sty_lugar"></div>
                    <div class="timeago sty_tiempo "></div>
                </div>
            </div>
            <div
                class="noticia_bottom flex flex-row w-full justify-between gap-12 pt-2 pb-0 max-[800px]:grid max-[800px]:grid-cols-1 max-[800px]:pt-2">
                <div class="noticia_btm_left">
                    <div class="autor max-w-[50ch] font-lora font-light text-[15px] text-zinc-800 max-[800px]:text-[14px]">
                    </div>
                    <div class="autor font-sf font-light text-[13px] pt-4 text-zinc-400 animate-pulse max-[800px]:pt-10">
                        Escrita por Miguel Gómez </div>
                </div>
                <div class="noticia_btm_right max-h-[500px] max-[800px]:max-w-[800px] max-[800px]:justify-items-center">
                    <img src="" alt="imagen de la noticia" class=" max-h-[500px] max-[800px]:max-w-[325px]">
                </div>

            </div>
        </div>
    </div>

    <div id="9"
        class="noticia border-l-1 border-r-1 border-t-0 border-black border max-[800px]:max-w-[800px] max-[800px]:border-r-0 max-[800px]:border-b-1 max-[800px]:border-l-0">
        <div class="noticia_holder">
            <div class="noticia_top">
                <div class="titular sty_titular"></div>
                <div class="subtitulo sty_subtitulo"></div>
                <div class="top_info">
                    <div class="lugar sty_lugar"></div>
                    <div class="timeago sty_tiempo "></div>
                </div>
            </div>
            <div
                class="noticia_bottom flex flex-row w-full justify-between gap-12 pt-2 pb-0 max-[800px]:grid max-[800px]:grid-cols-1 max-[800px]:pt-2">
                <div class="noticia_btm_left">
                    <div class="autor max-w-[50ch] font-lora font-light text-[15px] text-zinc-800 max-[800px]:text-[14px]">
                    </div>
                    <div class="autor font-sf font-light text-[13px] pt-4 text-zinc-400 animate-pulse max-[800px]:pt-10">
                        Escrita por Miguel Gómez </div>
                </div>
                <div class="noticia_btm_right max-h-[500px] max-[800px]:max-w-[800px] max-[800px]:justify-items-center">
                    <img src="" alt="imagen de la noticia" class=" max-h-[500px] max-[800px]:max-w-[325px]">
                </div>

            </div>
        </div>
    </div>

    <div id="10"
        class="noticia border-l-1 border-r-1 border-t-0 border-black border max-[800px]:max-w-[800px] max-[800px]:border-r-0 max-[800px]:border-b-1 max-[800px]:border-l-0">
        <div class="noticia_holder">
            <div class="noticia_top">
                <div class="titular sty_titular"></div>
                <div class="subtitulo sty_subtitulo"></div>
                <div class="top_info">
                    <div class="lugar sty_lugar"></div>
                    <div class="timeago sty_tiempo "></div>
                </div>
            </div>
            <div
                class="noticia_bottom flex flex-row w-full justify-between gap-12 pt-2 pb-0 max-[800px]:grid max-[800px]:grid-cols-1 max-[800px]:pt-2">
                <div class="noticia_btm_left">
                    <div class="autor max-w-[50ch] font-lora font-light text-[15px] text-zinc-800 max-[800px]:text-[14px]">
                    </div>
                    <div class="autor font-sf font-light text-[13px] pt-4 text-zinc-400 animate-pulse max-[800px]:pt-10">
                        Escrita por Miguel Gómez </div>
                </div>
                <div class="noticia_btm_right max-h-[500px] max-[800px]:max-w-[800px] max-[800px]:justify-items-center">
                    <img src="" alt="imagen de la noticia" class=" max-h-[500px] max-[800px]:max-w-[325px]">
                </div>

            </div>
        </div>
    </div>

    <div id="11"
        class="noticia border-l-1 border-r-1 border-t-0 border-black border max-[800px]:max-w-[800px] max-[800px]:border-r-0 max-[800px]:border-b-1 max-[800px]:border-l-0">
        <div class="noticia_holder">
            <div class="noticia_top">
                <div class="titular sty_titular"></div>
                <div class="subtitulo sty_subtitulo"></div>
                <div class="top_info">
                    <div class="lugar sty_lugar"></div>
                    <div class="timeago sty_tiempo "></div>
                </div>
            </div>
            <div
                class="noticia_bottom flex flex-row w-full justify-between gap-12 pt-2 pb-0 max-[800px]:grid max-[800px]:grid-cols-1 max-[800px]:pt-2">
                <div class="noticia_btm_left">
                    <div class="autor max-w-[50ch] font-lora font-light text-[15px] text-zinc-800 max-[800px]:text-[14px]">
                    </div>
                    <div class="autor font-sf font-light text-[13px] pt-4 text-zinc-400 animate-pulse max-[800px]:pt-10">
                        Escrita por Miguel Gómez </div>
                </div>
                <div class="noticia_btm_right max-h-[500px] max-[800px]:max-w-[800px] max-[800px]:justify-items-center">
                    <img src="" alt="imagen de la noticia" class=" max-h-[500px] max-[800px]:max-w-[325px]">
                </div>

            </div>
        </div>
    </div>

    <div id="12"
        class="noticia border-l-1 border-r-1 border-t-0 border-black border max-[800px]:max-w-[800px] max-[800px]:border-r-0 max-[800px]:border-b-1 max-[800px]:border-l-0">
        <div class="noticia_holder">
            <div class="noticia_top">
                <div class="titular sty_titular"></div>
                <div class="subtitulo sty_subtitulo"></div>
                <div class="top_info">
                    <div class="lugar sty_lugar"></div>
                    <div class="timeago sty_tiempo "></div>
                </div>
            </div>
            <div
                class="noticia_bottom flex flex-row w-full justify-between gap-12 pt-2 pb-0 max-[800px]:grid max-[800px]:grid-cols-1 max-[800px]:pt-2">
                <div class="noticia_btm_left">
                    <div class="autor max-w-[50ch] font-lora font-light text-[15px] text-zinc-800 max-[800px]:text-[14px]">
                    </div>
                    <div class="autor font-sf font-light text-[13px] pt-4 text-zinc-400 animate-pulse max-[800px]:pt-10">
                        Escrita por Miguel Gómez </div>
                </div>
                <div class="noticia_btm_right max-h-[500px] max-[800px]:max-w-[800px] max-[800px]:justify-items-center">
                    <img src="" alt="imagen de la noticia" class=" max-h-[500px] max-[800px]:max-w-[325px]">
                </div>

            </div>
        </div>
    </div> -->

    <!-- NOTICIA LONDRES BOMBA
        class="noticia border-l-1 border-r-1 border-t-0 border-black border max-[800px]:max-w-[800px] max-[800px]:border-r-0 max-[800px]:border-b-1 max-[800px]:border-l-0"
        v-show="isHidden">
        <div class="noticia_holder">
            <div class="noticia_top">
                <div class="titular sty_titular">Explosión en Londres: Atentado Sacude la Ciudad</div>
                <div class="subtitulo sty_subtitulo">En un desafortunado suceso, la capital británica fue sacudida por una
                    bomba que explotó en el corazón de la ciudad, dejando a su paso caos.</div>
                <div class="top_info">
                    <div class="lugar sty_lugar">Londres, Reino Unido</div>
                    <div class="timeago sty_tiempo ">HACE 2 HORAS</div>
                </div>
            </div>
            <div
                class="noticia_bottom flex flex-row w-full justify-between gap-12 pt-2 pb-0 max-[800px]:grid max-[800px]:grid-cols-1 max-[800px]:pt-2">
                <div class="noticia_btm_left">
                    <div class="autor max-w-[50ch] font-lora font-light text-[15px] text-zinc-800 max-[800px]:text-[14px]">
                        En un desafortunado suceso, la capital británica fue sacudida por una bomba que explotó en el
                        corazón de la ciudad, dejando a su paso caos y destrucción. <br><br>
                        El incidente ocurrió hoy por la mañana en una concurrida zona comercial, sembrando el pánico entre
                        los transeúntes y residentes cercanos. De acuerdo con las autoridades locales, la explosión, de
                        origen aún desconocido, tuvo lugar cerca de una estación de metro muy transitada y un conocido
                        centro comercial. Varios testigos relatan haber escuchado una fuerte detonación seguida de una nube
                        de humo y escombros.
                        <br><br>Inmediatamente, equipos de emergencia y servicios de seguridad llegaron al lugar para
                        socorrer a las víctimas y controlar la situación. Aunque aún no se han confirmado los detalles
                        exactos sobre el número de personas afectadas, se reportan múltiples heridos y posibles fallecidos.
                        Las autoridades están trabajando incansablemente para brindar asistencia médica y garantizar la
                        seguridad de todos los ciudadanos.
                    </div>
                    <div class="autor font-sf font-light text-[13px] pt-4 text-zinc-400 animate-pulse max-[800px]:pt-10">
                        escrita por {{ inputValue }} </div>
                </div>
                <div class="noticia_btm_right max-h-[500px] max-[800px]:max-w-[800px] max-[800px]:justify-items-center">
                    <img src="/noticias/imagen_noticia_vert.png" alt="imagen de la noticia"
                        class=" max-h-[500px] max-[800px]:max-w-[325px]">
                </div>

            </div>
        </div>
    </div> -->
    
    </template>




<script setup>

const { inputValue } = inject("inputData")
const isHidden = computed(() => {
    return inputValue.value != ""
})

</script>


<style lang="sass">
.noticia
    @apply p-8 pt-4 
    .noticia_holder
        @apply flex flex-col gap-6
        .noticia_top
            @apply flex flex-col gap-4 border-gris300_faux 
            border-bottom: solid 1px   
            .titular
                @apply text-3xl font-lora font-bold max-w-[40ch]
            .subtitulo
                @apply max-w-[105ch]
            .top_info
                @apply flex flex-col gap-2 pb-4
                
                .timeago
                    @apply animate-pulse
                    // font-family: 'SF UI Display'
                    // font-weight: normal
                    // font-size: 14px
                    // line-height: 16px
                    // color: #D95555

</style>