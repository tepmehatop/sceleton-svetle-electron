<script lang="ts">

    import {SlideToggle} from '@skeletonlabs/skeleton';

</script>

<div class="p-8">
    <div class="card p-10" slotPageContent="w-auto">
        <h4 class="pb-5">Генерация потребностей</h4>
        <div class="flex justify-end ...">
            <SlideToggle name="slider-large" active="bg-primary-500" size="sm" onclick="my_modal_2.showModal()">Хочу именную потребность</SlideToggle>
            <dialog id="my_modal_2" class="modal">
                <div class="modal-box">
                    <h3 class="font-bold text-lg">Введите свой токен для именной потребности</h3>
                    <textarea class="textarea" rows="4" placeholder="Введите свой токен" />
                    <button class="btn btn-success">Сохранить</button>
                    <button class="btn btn-error">Отменить</button>
                </div>
                <form method="dialog" class="modal-backdrop">
                    <button>close</button>
                </form>
            </dialog>

        </div>
        <div class="h-56 grid grid-cols-3 gap-4 content-start ...">
            <div>
                <select class="select select-info w-full max-w-xs">
                    <option disabled selected>Тип потребности</option>
                    <option>X86</option>
                    <option>X86+SHD</option>
                    <option>SHD</option>
                    <option>Виртуализация</option>
                </select>
            </div>
            <div>
                <div class="input-group input-group-divider grid-cols-[1fr_auto]">
                    <input type="text" placeholder="Введите количество" />
                    <pre class="pre">кол.</pre>
                </div>
            </div>
            <div>03</div>
            <div>04</div>
            <div>05</div>
        </div>

    </div>
</div>


<div class="container h-full mx-auto flex justify-center items-center">
    <div class="space-y-10 text-center flex flex-col items-center">
        <div class="flex justify-center space-x-2">
            <a href="/static" class="btn variant-filled">a</a>
            <button class="btn btn-active btn-neutral">Neutral</button>
            <button class="btn btn-info">Info</button>
            <button class="btn btn-success">
                <span class="loading loading-spinner"></span>
                loading</button>
            <button class="btn btn-warning">Warning</button>
            <button class="btn btn-warning">Warning</button>
            <button class="btn btn-error">Error</button>
            <div class="form-control">
                <label class="label cursor-pointer">
                    <span class="label-text">Remember me...</span>
                    <input type="checkbox" checked="checked" class="checkbox checkbox-primary" />
                </label>
            </div>
        </div>
    </div>
</div>
