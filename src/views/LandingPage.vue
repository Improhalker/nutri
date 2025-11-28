<template>
  <div class="fixed inset-0 w-full h-full bg-center bg-no-repeat bg-cover opacity-100 -z-10" style="background-image: url('/images/mainwallpaper.png');"></div>

  <div class="main-content flex flex-col justify-between min-h-[95svh] p-3 md:p-5 gap-4 md:gap-6">
    <!-- Header -->
    <div class="w-full z-[100] grid group-[.screen-mobile]:grid md:flex gap-3 md:gap-4 items-start md:justify-between">

      <!-- Logo mobile -->
      <div class="flex-1 flex items-start justify-between md:justify-start gap-4">
        <div class="block md:hidden mx-auto">
          <div class="w-[6rem] md:w-[8rem] aspect-square overflow-hidden relative">
            <img 
              src="https://media.inlead.cloud/uploads/40296/2025-10-22/md-YAUt8-logo8020-editado.png"
              alt="Imagem"
              class="absolute inset-0 w-full h-full object-cover"
            >
          </div>
        </div>
      </div>

      <!-- Logo desktop -->
      <div class="w-full grid gap-4 max-w-[28rem]">
        <div class="hidden md:block mx-auto">
          <div class="w-[6rem] md:w-[8rem] aspect-square relative overflow-hidden">
            <img 
              src="https://media.inlead.cloud/uploads/40296/2025-10-22/md-YAUt8-logo8020-editado.png"
              alt="Imagem"
              class="absolute inset-0 w-full h-full object-cover"
            >
          </div>
        </div>

        <!-- Barra progresso -->
        <div class="flex items-center gap-4">
          <div class="fixed top-0 left-0 w-full pt-2 z-[101] overflow-hidden">
            <div class="absolute inset-0 bg-featured opacity-10"></div>
            <div class="absolute inset-y-0 left-0 bg-featured ease duration-700" style="width: 3.44828%;"></div>
          </div>
        </div>
      </div>

      <div class="hidden md:block flex-1"></div>
    </div>

    <!-- Conteúdo -->
    <div class="w-full relative mx-auto max-w-[28rem]">
      <div class="flex flex-wrap -mx-[0.2rem]">

        <!-- Aviso -->
        <div class="px-[0.2rem] basis-full">
          <div class="grid bg-red-100 text-red-700 p-4 rounded-2xl">
            <p>⚠️ <u>ATENCIÓN</u>: ofrecemos 1 evaluación 80/20 por persona. <strong><u>Si salís ahora, perdés tu turno</u></strong>.</p>
          </div>
        </div>

        <!-- Texto principal -->
        <div class="px-[0.2rem] basis-full">
          <div class="py-2 break-words text-white">

            <!-- H1 principal 48px no mobile -->
            <h1 class="text-[48px] leading-tight text-center font-semibold">
              <span>Tu Dieta</span>
              <span class="text-green-600 font-bold"> Método 80/20 </span>
              <span>para bajar de peso 😊</span>
            </h1>

            <!-- Subtítulo -->
            <p class="text-center mt-2 text-lg">80% comidas del plan, 20% Gustos</p>

            <p class="text-center mt-2 text-lg">
              Usando tus respuestas, armamos una 
              <strong>dieta personalizada</strong> 
              justa <strong>PARA VOS</strong>, con recetas argentinas baratas 🙌
            </p>

            <!-- Lista de benefícios -->
            <div class="mt-4 space-y-1">
              <p class="font-bold text-[24px] flex items-start gap-2">
                <span class="text-green-400 text-[24px]">✅</span>
                Test GRATIS
              </p>

              <p class="font-bold text-[24px] flex items-start gap-2">
                <span class="text-green-400 text-[24px]">✅</span>
                Dieta 100% personalizada para bajar de peso
              </p>
            </div>

            <!-- H2 destacado -->
            <h2 class="mt-4 font-bold text-[24px] leading-tight">
              🌟 <span class="bg-green-600 px-2 rounded">APP EXCLUSIVA 80/20</span> AL FINAL DEL TEST
            </h2>

          </div>
        </div>


      <!-- Botão -->
        <div class="px-[0.2rem] mt-8 basis-full">
          <div class="mx-auto relative max-w-[28rem]">
            <div class="grid relative group/button">
              <!-- Efeito pulse -->
              <div 
                class="absolute inset-0 rounded-2xl bg-green-600 animate-pulse opacity-70 group-hover/button:opacity-90 transition">
              </div>
              <!-- Botão principal -->
              <button 
                onclick="window.location.href='/form'"
                class="relative rounded-2xl text-white font-semibold py-4 px-6 text-lg shadow-lg 
                hover:bg-green-800 hover:scale-[1.03] active:scale-[0.97] transition-all duration-200">
                CREAR MI DIETA EN 1 MINUTO
              </button>
            </div>
          </div>
        </div>

        <!-- Espaçamento -->
        <div class="px-[0.2rem] basis-full">
          <div class="h-4"></div>
        </div>
      </div>
    </div>
  <div class="py-10"></div>
</div>

</template>
