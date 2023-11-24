<style>
    .log-container {
        margin-top: 1em;
    }
</style>
<script>
  export const logs = [
    {
        time: "24.11.2024 13:01",
        buffer: "memory",
        topics: "l2tp, ppp ,info",
        message: "hello"
    },
    {
        time: "24.11.2024 13:01",
        buffer: "memory",
        topics: "l2tp, ppp ,info",
        message: "world"
    },
    {
        time: "24.11.2024 13:01",
        buffer: "memory",
        topics: "l2tp, ppp ,info",
        message: "haha!"
    }
];
</script> 

<div class="container log-container">
    <form>
        <fieldset>
            <label for="devises">Выбирите устройство</label>
            <select id="devises">
                <option value="0-13">0-13</option>
                <option value="14-17">14-17</option>
                <option value="18-23">18-23</option>
                <option value="24+">24+</option>
            </select>
            <label for="search">Поиск</label>
            <input type="text" placeholder="Введите текст для поиска" id="search">
            <button class="button">Поиск</button>
        </fieldset>
    </form>


    <table>
        <thead>
            <th>Время</th>
            <th>Буфер</th>
            <th>Службы</th>
            <th>Сообщение</th>
        </thead>
        <tbody>
            {#each logs as el}
                <tr>
                    <td>{el.time}</td>
                    <td>{el.buffer}</td>
                    <td>{el.topics}</td>
                    <td>{el.message}</td>
                </tr>
            {/each}
        </tbody>
    </table>
</div>
