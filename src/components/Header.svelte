<script>
    import tilt from "vanilla-tilt"
    import AccordianItem from "../components/AccordianItem.svelte"
</script>

<svelte:head>
    
</svelte:head>

<style>
	header {
		width: 100%;
		height: 800px;
	}
	.header-content {
		border-radius: 5px;
		background-image: url('https://res.cloudinary.com/daasu66it/image/upload/v1563908536/JamesBootHomepage/works/content/photo/codeykylie8.jpg');
		width: 100%;
		height: 100%;
		box-shadow: rgba(0, 0, 0, 0.12) 0 0 8px 0, rgba(0, 0, 0, 0.24) 0 4px 8px 0;
        padding: 2rem;
        color: azure;
        transform: perspective(1000px);
        transform-style: preserve-3d;
	}

    .header-title {
        transform: translateZ(20px)
    }

    .header-title h1 {
        vertical-align: middle;
        display: inline;
        font-family: effra, sans-serif;
        text-transform: uppercase;
        font-weight: 200;
    }
    .header-title p {
        vertical-align: middle;
        display: inline;
        font-family: effra, sans-serif;
        text-transform: uppercase;
        margin-left: 5px;
    }

    .profile-card {
        background-color: rgba(255,255,255,1);
        border-radius: 5px;
        padding: 5px;
    }

    .profile-card-header {
        margin-top: -18px;
        background-color: #d0542a;
        border-radius: 5px;
        font-family: effra;
        margin-right: 0;
        margin-left: auto;
        display: block;
        width: auto !important;
        padding: 5px;
        text-align: center;
    }
</style>

<header data-tilt data-tilt-perspective="1000" data-tilt-max="1">
	<div class="container h-100">
		<div class="row h-100">
			<div class="col-12 h-100 p-5">
                <div class="header-content">
                <div class="container-fluid">
                    <div class="row">
                        <div class="col-12 mb-5">
                            <div class="header-title">
                                <h1>James Zechman</h1><p>| Portfolio</p>
                            </div>
                        </div>
                        <div class="col-12 col-md-6 col-lg-3">
                            <div class="profile-card accordion accordion-flush" id="careersAccordian">
                                <div class="profile-card-header">
                                    <span>Employement</span>
                                </div>
                                <AccordianItem id="muv" title="Muv Ideas" content="Test Content" parent="careersAccordian" />
                                <AccordianItem id="jockey" title="Jockey" content="Test Content" parent="careersAccordian" />
                            </div>
                        </div>
                    </div>
                </div>
				
                    <!-- Add Slider for Images -->
                    
				</div>
			</div>
		</div>
	</div>
</header>