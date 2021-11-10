<div class="menu__wrap">
	<div class="menu__item">
		<a href="/">
			<img class="menu__logo" src="{logoMenu}" alt="{altLogo}">
		</a>
		<a href="{server_url}" class="button">Сервер</a>
	</div>
</div>
<div class="Page">
	<main>
		<about>
			<img class="logo_img" src="{logo}" alt="{altLogo}"/>
			<p>{name}</p>
			<h2>Серверов: {servers}</h2>
			<links>
				<ul>
					<li>
						<a class="btn" href="{invite_url}">Добавить бота</a>
					</li>
				</ul>
			</links>
		</about>
	</main>
</div>

<script>
	const name = "Anni\nДискорд бот!"
	const logoMenu = "https://cdn.discordapp.com/avatars/817889533345136640/f416309c263e2b75d1724ea66ed08874.webp?size=2048"
	const logo = "https://cdn.discordapp.com/avatars/817889533345136640/f416309c263e2b75d1724ea66ed08874.webp?size=2048"
	const altLogo = "Anni милаха"
	const servers = "1 500"
	const invite_url = "https://discord.com/oauth2/authorize?client_id=817889533345136640&scope=bot+applications.commands&permissions=8"
	const server_url = "https://discord.gg/PXa7SwnY5W"
</script>

<style>
	* {
		box-sizing: border-box;
	}

	a {
		text-decoration: none;
	}

	main {
    text-align: center;
    position: absolute;
    transform: translate(-50%,-50%);
    left: 50%;
    top: 40%;
	}
	
	p {
		color: #fff;
		font-size: 30px;
		font-weight: 100;
	}

	ul {
    padding-left: 0;
	}

	li {
		display: inline-block;
    margin-right: 5px;
    margin-left: 5px;
    width: auto;
	}

	.button {
		position: absolute;
		right: 20px;
    display: inline-flex;
    min-height: 32px;
    color: var(--color-primary,#ffffff);
    outline: 0;
    font-stretch: normal;
    font-weight: 600;
    font-size: 1.3rem;
	}
	.button:hover {
		color: rgba(202, 202, 202, 0.336);
		transition: color 0.2s linear;	
	}

	.Page {
		background-color: #23232a;
		box-shadow: var(--shadow-main,0 18px 36px rgba(0,0,0,.14));
		border-radius: 30px;
		height: 630px;
	}

	.btn {
		color: var(--color-btn-text);
    background-color: var(--color-btn-bg);
    border-color: var(--color-btn-border);
    box-shadow: var(--color-btn-shadow),var(--color-btn-inset-shadow);
    transition: .2s cubic-bezier(0.3, 0, 0.5, 1);
    transition-property: color,background-color,border-color;

		padding: 5px 16px;
		font-size: 14px;
    font-weight: 500;
    line-height: 20px;
    white-space: nowrap;
    vertical-align: middle;
    cursor: pointer;
		user-select: none;
    border: 1px solid;
    border-radius: 3px;
		text-decoration: none;
	}

	.btn:hover {
		color: #fff;
	}

	.logo_img {
    width: 128px;
    height: 128px;
    border-radius: 100%;
    pointer-events: none;
    margin: 0;
		border: 3px solid #ffffff;
    box-shadow: 0 0 15px black;
	}

	.menu__wrap {
		background-color: #1c1c22;
		box-shadow: 0 0 10px black;
		position: fixed;
    display: flex;
    top: 0;
    left: 0;
    right: 0;
    flex: 0 0 auto;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    height: 51px;
    padding: 5px 20px;
    box-sizing: border-box;
    z-index: 10;
	}

	.menu__item {
		display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-start;
    flex: 0 1 auto;
    min-width: 0;
    max-width: 100%;
	}

	.menu__logo {
    width: 40px;
    height: 40px;
    border-radius: 100%;
    pointer-events: none;
    margin: 0;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}

	/* Iphone 6/7/8 */
		@media (min-width: 375px) {
		main {
			max-width: none;
		}
	}
</style>