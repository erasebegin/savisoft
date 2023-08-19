<script>
	import logo from '../lib/images/savisoft-logo-with-text.svg';
</script>

<header class="header">
	<div class="header__logo">
		<img class="header__img" alt="header company logo" src={logo} />
	</div>

	<div class="header__menu">
		<nav id="navbar" class="header__nav collapse">
			<ul class="header__elenco">
				<li class="header__el"><a href="/">Home</a></li>
				<li class="header__el"><a href="/">Contact</a></li>
				<li class="header__el header__el--blue">
					<a href="" class="btn btn--white">SaviCase →</a>
				</li>
			</ul>
		</nav>
	</div>
</header>

<style lang="scss">
	.header {
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 30px 25px;

		&__logo img {
			max-height: 50px;
		}

		&__elenco {
			padding: 0;
			margin: 0;
			list-style: none;
		}

		&__menu {
			float: right;
		}

		&__el {
			padding: 0 25px;
			display: inline-block;

			a {
				text-decoration: none;
				color: #1f4568;
				font-size: 14px;
			}
		}

		&__img {
			display: inline-block;
			vertical-align: middle;
		}

		&__title {
			font-size: 18px;
			margin: 0;
			margin-left: 10px;
			display: inline-block;
			line-height: 18px;
			vertical-align: middle;
		}

		&__light {
			color: #8198ae;
		}

		&__link:hover {
			text-decoration: none;
			color: #3a9fff;
		}
	}

	@media screen and (max-width: 1024px) {
		.header {
			background-color: #fff;
			padding: 0;
			box-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
			position: fixed;
			top: 0;
			left: 0;
			width: 100%;
			z-index: 4;

			&__container {
				width: 100%;
				padding: 0;
			}

			&__logo {
				padding: 12px 20px 12px 20px;
			}

			&__menu {
				width: 100%;
			}

			&__el {
				display: block;
				padding: 10px 20px;
				border-top: 1px solid #ededed;
			}

			&__el--blue {
				background-color: #3a9fff;
			}

			.btn--white,
			.btn--white:hover {
				padding: 0;
				border: 0;
				box-shadow: none;
				color: #fff;
				background-color: transparent;
			}
		}
		.navbar-toggle {
			margin: 0;
			display: inline-block;
			margin-right: 10px;
			margin-top: 10px;
		}
	}
</style>
