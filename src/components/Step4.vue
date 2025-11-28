<template>
    <div class="w-full relative mx-auto max-w-[28rem]">

        <div class="flex flex-wrap -mx-1">

            <!-- TÍTULO -->
            <div class="w-full px-1">
                <h1 class="text-center text-xl md:text-2xl font-semibold leading-tight">
                    ¿Habías probado dietas para
                    <span class="text-green-600 font-bold">bajar de peso</span>?
                </h1>
                <p class="text-center mt-1 text-sm opacity-90">Elegí una opción</p>
            </div>

            <!-- OPÇÕES -->
            <div class="w-full px-1 mt-4">

                <div class="grid grid-cols-2 gap-2">

                    <!-- SIM -->
                    <button
                        class="group option-theme rounded-2xl overflow-hidden border bg-white/90 active:scale-[.98] transition shadow-sm">
                        <div class="flex items-center justify-center p-3 min-h-[56px]">
                            <p class="text-center text-gray-800 text-base font-medium">
                                ✅ Sí
                            </p>
                        </div>
                    </button>

                    <!-- NÃO -->
                    <button
                        class="group option-theme rounded-2xl overflow-hidden border bg-white/90 active:scale-[.98] transition shadow-sm">
                        <div class="flex items-center justify-center p-3 min-h-[56px]">
                            <p class="text-center text-gray-800 text-base font-medium">
                                🚫 No
                            </p>
                        </div>
                    </button>

                </div>

            </div>

        </div>
    </div>

</template>