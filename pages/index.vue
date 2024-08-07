<template>
    <main class="h-full flex flex-col gap-4" id="main">
			<div class="bg-hh-base md:rounded-lg w-full mx-auto flex grow md:grow-0">
				<div class="flex flex-col md:flex-row gap-8 w-full pb-8" id="wrapperContent">
					<div class="w-full flex rounded-lg relative flex-col grow" id="primaryContent">
						<div class="flex flex-col rounded-lg relative mb-8">
							<div class="h-64 w-full">
								<img src="~/assets/Garden.webp" alt="Grand Punta Cana" data-gallery-id="0" data-large-image="https://cdn.holidayhero.com/listing_headers/ad8937ca-ed7a-4d86-9757-4cda8fc6551a/gerson-repreza-CepDpEiALqM-unsplash_1.jpg?width=1000&amp;height=625&amp;fit=bounds&amp;format=webp" class="galleryImage h-64 md:rounded-tr-lg md:rounded-tl-lg w-full object-cover object-center">
							</div>
							<div class="-mt-24 z-10 ml-8">
								<img src="~/assets/Logo.png" alt="" class="rounded-full w-12 h-12 bg-hh-base90 object-cover object-bottom border-4 border-hh-base90">
							</div>
							<div class="-mt-6 mx-4 rounded-lg bg-hh-base90 h-auto pb-2 text-hh-on-base px-2 sm:px4">
								<div class="flex flex-row">
									<div class="w-5/6 ml-2">
										<div class="flex flex-col gap-1 my-7">
											<div class="text-lg text-hh-on-base font-medium tracking-tight leading-normal">
												ZenSakura Tuinhuis
											</div>
											<div class="text-md text-hh-base30 leading-tight line-clamp-1">
												Borne, Woolderweg 87
											</div>
											<div class="mt-2 flex md:flex-row gap-4 pr-2">
												<button class="grow-0 rounded-full text-sm bg-hh-base60 text-fullwhite px-4 py-2 font-bold showMyStay" aria-label="My Stay">My Stay</button>
												<button class="grow-0 rounded-full text-sm bg-hh-base60 text-hh-on-base px-2 py-2 w-10 h-10 showDirections showModal" data-modal="directions" aria-label="Get Directions">
													<svg width="16" height="18" viewBox="0 0 16 18" xmlns="http://www.w3.org/2000/svg" class="mx-auto fill-hh-on-base">
														<path fill-rule="evenodd" clip-rule="evenodd" d="M8.00065 0.875C3.97982 0.875 0.708984 4.14583 0.708984 8.16667C0.708984 12.4311 4.62213 15.016 7.21214 16.7268L7.21315 16.7275L7.65398 17.02C7.75898 17.09 7.87982 17.125 8.00065 17.125C8.12148 17.125 8.24232 17.09 8.34732 17.02L8.78816 16.7275L8.78916 16.7268C11.3792 15.016 15.2923 12.4311 15.2923 8.16667C15.2923 4.14583 12.0215 0.875 8.00065 0.875ZM8.00065 10.6667C9.38136 10.6667 10.5007 9.54738 10.5007 8.16667C10.5007 6.78595 9.38136 5.66667 8.00065 5.66667C6.61994 5.66667 5.50065 6.78595 5.50065 8.16667C5.50065 9.54738 6.61994 10.6667 8.00065 10.6667Z"></path>
													</svg>
												</button>
												<button class="grow-0 rounded-full text-sm bg-hh-base60 text-hh-on-base px-2 py-2 w-10 h-10 showContactHost showModal" data-modal="contactHost" aria-label="Contact Host">
													<svg width="16" height="13" viewBox="0 0 16 13" xmlns="http://www.w3.org/2000/svg" class="mx-auto fill-hh-on-base">
														<path d="M7.17016 12.551L15.5075 1.40523C15.8935 0.886092 15.4756 0.162287 14.833 0.236988L1.01179 1.88444C0.486444 1.94225 0.202574 2.52096 0.462838 2.97175L2.14637 5.90238C2.32966 6.21984 2.7222 6.35722 3.06165 6.21203L12.7258 2.2324L4.44362 8.60567C4.15182 8.8334 4.07453 9.24204 4.25781 9.5595L5.95404 12.4828C6.21431 12.9336 6.85742 12.9771 7.17016 12.551Z"></path>
													</svg>
												</button>
											</div>
										</div>
									</div>
									<div class="bg-hh-base !h-20 text-hh-on-base rounded-br-lg rounded-bl-lg pt-0 text-center px-2 py-1">
										<div class="mt-2 px-1">
											<p class="text-xs uppercase font-medium mb-2">
												Temp
											</p>
											<p class="text-hh-bas">
												<p id="temprature"></p>
											</p>
										</div>
									</div>
								</div>
							</div>
						</div>
						<div class="px-4 grow">
							<!--- Start Main Content -->
							<div class="flex flex-col w-full gap-8 pb-8">
								<!-- Start Announcements -->
								<div class="flex flex-col">
									<div class="flex gap-4 flex-nowrap overflow-x-auto no-scrollbar snap-x">
										<div class="flex-none w-80 min-h-48 h-auto snap-start relative" id="announcement_258571553124607168">
											<div class="absolute w-8 h-8 top-2 right-2 rounded-full bg-hh-base30 flex items-center cursor-pointer hideAnnouncement" data-announcement-id="258571553124607168">
												<svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="fill-hh-base mx-auto w-6 h-6">
													<path d="M18.5297 17.4698C18.8227 17.7628 18.8227 18.2378 18.5297 18.5308C18.3837 18.6768 18.1917 18.7508 17.9997 18.7508C17.8077 18.7508 17.6158 18.6778 17.4698 18.5308L11.9997 13.0608L6.52975 18.5308C6.38375 18.6768 6.19175 18.7508 5.99975 18.7508C5.80775 18.7508 5.61575 18.6778 5.46975 18.5308C5.17675 18.2378 5.17675 17.7628 5.46975 17.4698L10.9398 11.9998L5.46975 6.52981C5.17675 6.23681 5.17675 5.76177 5.46975 5.46877C5.76275 5.17577 6.23775 5.17577 6.53075 5.46877L12.0008 10.9388L17.4707 5.46877C17.7637 5.17577 18.2387 5.17577 18.5317 5.46877C18.8247 5.76177 18.8247 6.23681 18.5317 6.52981L13.0617 11.9998L18.5297 17.4698Z"></path>
												</svg>
											</div>
											<div class="w-full h-full flex flex-col gap-2 p-5 justify-between bg-hh-base90 rounded-xl bg-gradient-to-tr from-hh-base90 to-hh-card-even">
												<div>
													<p class="text-2xl font-semibold text-hh-on-base line-clamp-2 mb-2">Connect to the WiFi</p>
													<p class="text-sm text-hh-on-base leading-7 font-normal">Network: PuntaCana<br>
														Password: X2n(koyu
													</p>
												</div>
												<div class="flex flex-row gap-4 mt-1">
													<div class="flex-none">
														<a href="" class="block px-4 py-2 bg-hh-secondary text-sm font-bold text-hh-on-secondary rounded-full leading-normal tracking-wide">Connect</a>
													</div>
													<div class="w-9 h-9 rounded-full bg-hh-secondary flex items-center cursor-pointer copyToClipboard" data-copy-value="123445">
														<svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg" class="mx-auto w-4 h-4">
															<path d="M17.1083 6.225L12.9416 2.05833C12.8241 1.94083 12.6658 1.875 12.4999 1.875H8.6665C6.99817 1.875 6.04159 2.83166 6.04159 4.5V5.20833H5.33317C3.66484 5.20833 2.70825 6.165 2.70825 7.83333V16.3333C2.70825 18.0008 3.66484 18.9583 5.33317 18.9583H11.3325C13.0009 18.9583 13.9574 18.0017 13.9574 16.3333V15.625H14.6659C16.3342 15.625 17.2908 14.6683 17.2908 13V6.66667C17.2916 6.50083 17.2258 6.34167 17.1083 6.225ZM13.1249 4.00917L15.1574 6.04167H14.5833C13.5333 6.04167 13.1249 5.6325 13.1249 4.58333V4.00917ZM12.7083 16.3333C12.7083 17.3225 12.3225 17.7083 11.3333 17.7083H5.33398C4.34398 17.7083 3.95907 17.3225 3.95907 16.3333V7.83333C3.95907 6.84416 4.34482 6.45833 5.33398 6.45833H6.0424V13C6.0424 14.6675 6.99898 15.625 8.66732 15.625H12.7091V16.3333H12.7083ZM14.6667 14.375H8.66732C7.67732 14.375 7.2924 13.9892 7.2924 13V4.5C7.2924 3.51083 7.67815 3.125 8.66732 3.125H11.8757V4.58333C11.8757 6.33 12.8374 7.29167 14.5841 7.29167H16.0424V13C16.0416 13.9892 15.6558 14.375 14.6667 14.375Z" fill="#0c111e"></path>
														</svg>
													</div>
												</div>
											</div>
										</div>
										<div class="flex-none w-80 min-h-48 h-auto snap-start relative" id="announcement_258585127519740352">
											<div class="absolute w-8 h-8 top-2 right-2 rounded-full bg-hh-base30 flex items-center cursor-pointer hideAnnouncement" data-announcement-id="258585127519740352">
												<svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="fill-hh-base mx-auto w-6 h-6">
													<path d="M18.5297 17.4698C18.8227 17.7628 18.8227 18.2378 18.5297 18.5308C18.3837 18.6768 18.1917 18.7508 17.9997 18.7508C17.8077 18.7508 17.6158 18.6778 17.4698 18.5308L11.9997 13.0608L6.52975 18.5308C6.38375 18.6768 6.19175 18.7508 5.99975 18.7508C5.80775 18.7508 5.61575 18.6778 5.46975 18.5308C5.17675 18.2378 5.17675 17.7628 5.46975 17.4698L10.9398 11.9998L5.46975 6.52981C5.17675 6.23681 5.17675 5.76177 5.46975 5.46877C5.76275 5.17577 6.23775 5.17577 6.53075 5.46877L12.0008 10.9388L17.4707 5.46877C17.7637 5.17577 18.2387 5.17577 18.5317 5.46877C18.8247 5.76177 18.8247 6.23681 18.5317 6.52981L13.0617 11.9998L18.5297 17.4698Z"></path>
												</svg>
											</div>
											<div class="w-full h-full flex flex-col gap-2 p-5 justify-between bg-hh-base90 rounded-xl bg-gradient-to-tr from-hh-base90 to-hh-card-even">
												<div>
													<p class="text-2xl font-semibold text-hh-on-base line-clamp-2 mb-2">Rebook for next year</p>
													<p class="text-sm text-hh-on-base leading-7 font-normal">And get a 15% discount</p>
												</div>
												<div class="flex flex-row gap-4 mt-1">
													<div class="flex-none">
														<a href="" target="&quot;_blank&quot;" class="block px-4 py-2 bg-hh-secondary text-sm font-bold text-hh-on-secondary rounded-full leading-normal tracking-wide">Claim discount</a>
													</div>
												</div>
											</div>
										</div>
										<div class="flex-none w-80 min-h-48 h-auto snap-start relative" id="announcement_269787904996501184">
											<div class="absolute w-8 h-8 top-2 right-2 rounded-full bg-hh-base30 flex items-center cursor-pointer hideAnnouncement" data-announcement-id="269787904996501184">
												<svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="fill-hh-base mx-auto w-6 h-6">
													<path d="M18.5297 17.4698C18.8227 17.7628 18.8227 18.2378 18.5297 18.5308C18.3837 18.6768 18.1917 18.7508 17.9997 18.7508C17.8077 18.7508 17.6158 18.6778 17.4698 18.5308L11.9997 13.0608L6.52975 18.5308C6.38375 18.6768 6.19175 18.7508 5.99975 18.7508C5.80775 18.7508 5.61575 18.6778 5.46975 18.5308C5.17675 18.2378 5.17675 17.7628 5.46975 17.4698L10.9398 11.9998L5.46975 6.52981C5.17675 6.23681 5.17675 5.76177 5.46975 5.46877C5.76275 5.17577 6.23775 5.17577 6.53075 5.46877L12.0008 10.9388L17.4707 5.46877C17.7637 5.17577 18.2387 5.17577 18.5317 5.46877C18.8247 5.76177 18.8247 6.23681 18.5317 6.52981L13.0617 11.9998L18.5297 17.4698Z"></path>
												</svg>
											</div>
											<div class="w-full h-full flex flex-col gap-2 p-5 justify-between bg-hh-base90 rounded-xl bg-gradient-to-tr from-hh-base90 to-hh-card-odd">
												<div>
													<p class="text-2xl font-semibold text-hh-on-base line-clamp-2 mb-2">Welkomst video</p>
													<p class="text-sm text-hh-on-base leading-7 font-normal">Kijk nu de welkomst video</p>
												</div>
												<div class="flex flex-row gap-4 mt-1">
													<div class="flex-none">
														<a href="" target="&quot;_blank&quot;" class="block px-4 py-2 bg-hh-secondary text-sm font-bold text-hh-on-secondary rounded-full leading-normal tracking-wide">kijk nu</a>
													</div>
												</div>
											</div>
										</div>
										<div class="flex-none w-80 min-h-48 h-auto snap-start relative" id="announcement_318747191122551616">
											<div class="absolute w-8 h-8 top-2 right-2 rounded-full bg-hh-base30 flex items-center cursor-pointer hideAnnouncement" data-announcement-id="318747191122551616">
												<svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="fill-hh-base mx-auto w-6 h-6">
													<path d="M18.5297 17.4698C18.8227 17.7628 18.8227 18.2378 18.5297 18.5308C18.3837 18.6768 18.1917 18.7508 17.9997 18.7508C17.8077 18.7508 17.6158 18.6778 17.4698 18.5308L11.9997 13.0608L6.52975 18.5308C6.38375 18.6768 6.19175 18.7508 5.99975 18.7508C5.80775 18.7508 5.61575 18.6778 5.46975 18.5308C5.17675 18.2378 5.17675 17.7628 5.46975 17.4698L10.9398 11.9998L5.46975 6.52981C5.17675 6.23681 5.17675 5.76177 5.46975 5.46877C5.76275 5.17577 6.23775 5.17577 6.53075 5.46877L12.0008 10.9388L17.4707 5.46877C17.7637 5.17577 18.2387 5.17577 18.5317 5.46877C18.8247 5.76177 18.8247 6.23681 18.5317 6.52981L13.0617 11.9998L18.5297 17.4698Z"></path>
												</svg>
											</div>
											<div class="w-full h-full flex flex-col gap-2 p-5 justify-between bg-hh-base90 rounded-xl bg-gradient-to-tr from-hh-base90 to-hh-card-even">
												<div>
													<p class="text-2xl font-semibold text-hh-on-base line-clamp-2 mb-2">massage</p>
													<p class="text-sm text-hh-on-base leading-7 font-normal">boek nu een massage met 10% korting</p>
												</div>
												<div class="flex flex-row gap-4 mt-1">
													<div class="flex-none">
														<a href="" target="&quot;_blank&quot;" class="block px-4 py-2 bg-hh-secondary text-sm font-bold text-hh-on-secondary rounded-full leading-normal tracking-wide">Reserveer nu</a>
													</div>
												</div>
											</div>
										</div>
										<div class="flex-none w-80 min-h-48 h-auto snap-start relative" id="announcement_323771071927118208">
											<div class="absolute w-8 h-8 top-2 right-2 rounded-full bg-hh-base30 flex items-center cursor-pointer hideAnnouncement" data-announcement-id="323771071927118208">
												<svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="fill-hh-base mx-auto w-6 h-6">
													<path d="M18.5297 17.4698C18.8227 17.7628 18.8227 18.2378 18.5297 18.5308C18.3837 18.6768 18.1917 18.7508 17.9997 18.7508C17.8077 18.7508 17.6158 18.6778 17.4698 18.5308L11.9997 13.0608L6.52975 18.5308C6.38375 18.6768 6.19175 18.7508 5.99975 18.7508C5.80775 18.7508 5.61575 18.6778 5.46975 18.5308C5.17675 18.2378 5.17675 17.7628 5.46975 17.4698L10.9398 11.9998L5.46975 6.52981C5.17675 6.23681 5.17675 5.76177 5.46975 5.46877C5.76275 5.17577 6.23775 5.17577 6.53075 5.46877L12.0008 10.9388L17.4707 5.46877C17.7637 5.17577 18.2387 5.17577 18.5317 5.46877C18.8247 5.76177 18.8247 6.23681 18.5317 6.52981L13.0617 11.9998L18.5297 17.4698Z"></path>
												</svg>
											</div>
											<div class="w-full h-full flex flex-col gap-2 p-5 justify-between bg-hh-base90 rounded-xl bg-gradient-to-tr from-hh-base90 to-hh-card-odd">
												<div>
													<p class="text-2xl font-semibold text-hh-on-base line-clamp-2 mb-2">book now for next year</p>
													<p class="text-sm text-hh-on-base leading-7 font-normal">book now!</p>
												</div>
												<div class="flex flex-row gap-4 mt-1">
													<div class="flex-none">
														<a href="" target="&quot;_blank&quot;" class="block px-4 py-2 bg-hh-secondary text-sm font-bold text-hh-on-secondary rounded-full leading-normal tracking-wide">Book now with free breakfast</a>
													</div>
												</div>
											</div>
										</div>
										<div class="flex-none w-80 min-h-48 h-auto snap-start relative" id="announcement_338241761933746688">
											<div class="absolute w-8 h-8 top-2 right-2 rounded-full bg-hh-base30 flex items-center cursor-pointer hideAnnouncement" data-announcement-id="338241761933746688">
												<svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="fill-hh-base mx-auto w-6 h-6">
													<path d="M18.5297 17.4698C18.8227 17.7628 18.8227 18.2378 18.5297 18.5308C18.3837 18.6768 18.1917 18.7508 17.9997 18.7508C17.8077 18.7508 17.6158 18.6778 17.4698 18.5308L11.9997 13.0608L6.52975 18.5308C6.38375 18.6768 6.19175 18.7508 5.99975 18.7508C5.80775 18.7508 5.61575 18.6778 5.46975 18.5308C5.17675 18.2378 5.17675 17.7628 5.46975 17.4698L10.9398 11.9998L5.46975 6.52981C5.17675 6.23681 5.17675 5.76177 5.46975 5.46877C5.76275 5.17577 6.23775 5.17577 6.53075 5.46877L12.0008 10.9388L17.4707 5.46877C17.7637 5.17577 18.2387 5.17577 18.5317 5.46877C18.8247 5.76177 18.8247 6.23681 18.5317 6.52981L13.0617 11.9998L18.5297 17.4698Z"></path>
												</svg>
											</div>
											<div class="w-full h-full flex flex-col gap-2 p-5 justify-between bg-hh-base90 rounded-xl bg-gradient-to-tr from-hh-base90 to-hh-card-even">
												<div>
													<p class="text-2xl font-semibold text-hh-on-base line-clamp-2 mb-2">Follow us on insta</p>
													<p class="text-sm text-hh-on-base leading-7 font-normal">Follow us on insta</p>
												</div>
												<div class="flex flex-row gap-4 mt-1">
													<div class="flex-none">
														<a href="" target="&quot;_blank&quot;" class="block px-4 py-2 bg-hh-secondary text-sm font-bold text-hh-on-secondary rounded-full leading-normal tracking-wide">follow now!</a>
													</div>
												</div>
											</div>
										</div>
										<div class="flex-none w-80 min-h-48 h-auto snap-start relative" id="announcement_339413390319641664">
											<div class="absolute w-8 h-8 top-2 right-2 rounded-full bg-hh-base30 flex items-center cursor-pointer hideAnnouncement" data-announcement-id="339413390319641664">
												<svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="fill-hh-base mx-auto w-6 h-6">
													<path d="M18.5297 17.4698C18.8227 17.7628 18.8227 18.2378 18.5297 18.5308C18.3837 18.6768 18.1917 18.7508 17.9997 18.7508C17.8077 18.7508 17.6158 18.6778 17.4698 18.5308L11.9997 13.0608L6.52975 18.5308C6.38375 18.6768 6.19175 18.7508 5.99975 18.7508C5.80775 18.7508 5.61575 18.6778 5.46975 18.5308C5.17675 18.2378 5.17675 17.7628 5.46975 17.4698L10.9398 11.9998L5.46975 6.52981C5.17675 6.23681 5.17675 5.76177 5.46975 5.46877C5.76275 5.17577 6.23775 5.17577 6.53075 5.46877L12.0008 10.9388L17.4707 5.46877C17.7637 5.17577 18.2387 5.17577 18.5317 5.46877C18.8247 5.76177 18.8247 6.23681 18.5317 6.52981L13.0617 11.9998L18.5297 17.4698Z"></path>
												</svg>
											</div>
											<div class="w-full h-full flex flex-col gap-2 p-5 justify-between bg-hh-base90 rounded-xl bg-gradient-to-tr from-hh-base90 to-hh-card-odd">
												<div>
													<p class="text-2xl font-semibold text-hh-on-base line-clamp-2 mb-2">open the door</p>
												</div>
												<div class="flex flex-row gap-4 mt-1">
													<div class="flex-none">
														<a href="" class="block px-4 py-2 bg-hh-secondary text-sm font-bold text-hh-on-secondary rounded-full leading-normal tracking-wide">open now</a>
													</div>
												</div>
											</div>
										</div>
										<div class="flex-none w-80 min-h-48 h-auto snap-start relative" id="announcement_340801328890735296">
											<div class="absolute w-8 h-8 top-2 right-2 rounded-full bg-hh-base30 flex items-center cursor-pointer hideAnnouncement" data-announcement-id="340801328890735296">
												<svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="fill-hh-base mx-auto w-6 h-6">
													<path d="M18.5297 17.4698C18.8227 17.7628 18.8227 18.2378 18.5297 18.5308C18.3837 18.6768 18.1917 18.7508 17.9997 18.7508C17.8077 18.7508 17.6158 18.6778 17.4698 18.5308L11.9997 13.0608L6.52975 18.5308C6.38375 18.6768 6.19175 18.7508 5.99975 18.7508C5.80775 18.7508 5.61575 18.6778 5.46975 18.5308C5.17675 18.2378 5.17675 17.7628 5.46975 17.4698L10.9398 11.9998L5.46975 6.52981C5.17675 6.23681 5.17675 5.76177 5.46975 5.46877C5.76275 5.17577 6.23775 5.17577 6.53075 5.46877L12.0008 10.9388L17.4707 5.46877C17.7637 5.17577 18.2387 5.17577 18.5317 5.46877C18.8247 5.76177 18.8247 6.23681 18.5317 6.52981L13.0617 11.9998L18.5297 17.4698Z"></path>
												</svg>
											</div>
											<div class="w-full h-full flex flex-col gap-2 p-5 justify-between bg-hh-base90 rounded-xl bg-gradient-to-tr from-hh-base90 to-hh-card-even">
												<div>
													<p class="text-2xl font-semibold text-hh-on-base line-clamp-2 mb-2">belangrijke informatie</p>
												</div>
												<div class="flex flex-row gap-4 mt-1">
													<div class="flex-none">
														<a href="" class="block px-4 py-2 bg-hh-secondary text-sm font-bold text-hh-on-secondary rounded-full leading-normal tracking-wide">kijk nu</a>
													</div>
												</div>
											</div>
										</div>
									</div>
								</div>
								<!-- End Announcements -->
								<!-- Start Recommendations -->
								<div class="flex flex-col">
									<div class="flex flex-row justify-between">
										<div>
											<p class="text-lg font-semibold text-hh-on-base leading-normal tracking-wider">
												Recommendations
											</p>
										</div>
										<div>
											<a href="" aria-label="View all recommendations">
												<p class="text-sm font-semibold text-hh-on-base leading-normal tracking-wide">
													View all
												</p>
											</a>
										</div>
									</div>
									<div class="flex flex-row gap-2 my-4 overflow-x-scroll no-scrollbar snap-x">
										<div class="flex-none snap-start">
											<a href="" class="rounded-full bg-hh-base80 text-hh-base30 text-sm px-4 py-2 block">
											<span class="mr-2">🏰</span>
											<span>Attractions</span>
											</a>
										</div>
										<div class="flex-none snap-start">
											<a href="" class="rounded-full bg-hh-base80 text-hh-base30 text-sm px-4 py-2 block">
											<span class="mr-2">🏄🏻‍</span>
											<span>Tours &amp; activities</span>
											</a>
										</div>
										<div class="flex-none snap-start">
											<a href="" class="rounded-full bg-hh-base80 text-hh-base30 text-sm px-4 py-2 block">
											<span class="mr-2">🏖️</span>
											<span>Beaches</span>
											</a>
										</div>
										<div class="flex-none snap-start">
											<a href="" class="rounded-full bg-hh-base80 text-hh-base30 text-sm px-4 py-2 block">
											<span class="mr-2">🍔</span>
											<span>Food &amp; Drink</span>
											</a>
										</div>
									</div>
									<div class="flex flex-row gap-4 mt-2 overflow-x-auto no-scrollbar snap-x">
										<div class="flex-none snap-start">
											<a href="" aria-label="The Three Eyes National Park">
												<div class="w-40 h-auto flex flex-col gap-2">
													<img src="https://cdn.holidayhero.com/experience_images/6f1eceac-ef8d-42ab-bc1a-c89a01b35afd/photo.jpg?width=1000&amp;format=webp" alt="The Three Eyes National Park" class="w-40 h-64 rounded-lg object-cover object-center">
													<p class="text-hh-base text-hh-on-base text-">The Three Eyes National Park</p>
													<p class="text-md text-hh-base30 font-normal line-clamp-2">
														Santo Domingo Este
													</p>
												</div>
											</a>
										</div>
										<div class="flex-none snap-start">
											<a href="" aria-label="Saona Island">
												<div class="w-40 h-auto flex flex-col gap-2">
													<img src="https://cdn.holidayhero.com/experience_images/d5dc01e2-ce0f-428e-90e3-6025234ce1cf/DominicanRepublic-scaled.jpg?width=1000&amp;format=webp" alt="Saona Island" class="w-40 h-64 rounded-lg object-cover object-center">
													<p class="text-hh-base text-hh-on-base text-">Saona Island</p>
													<p class="text-md text-hh-base30 font-normal line-clamp-2">
														Punta Cana
													</p>
												</div>
											</a>
										</div>
										<div class="flex-none snap-start">
											<a href="" aria-label="JellyFish Restaurant">
												<div class="w-40 h-auto flex flex-col gap-2">
													<img src="https://cdn.holidayhero.com/experience_images/d6e365b6-c471-4dac-903c-9d6e39ee5d20/Screenshot_2023-12-15_at_13.46.51.png?width=1000&amp;format=webp" alt="JellyFish Restaurant" class="w-40 h-64 rounded-lg object-cover object-center">
													<p class="text-hh-base text-hh-on-base text-">JellyFish Restaurant</p>
												</div>
											</a>
										</div>
										<div class="flex-none snap-start">
											<a href="" aria-label="Horseback riding">
												<div class="w-40 h-auto flex flex-col gap-2">
													<img src="https://cdn.holidayhero.com/experience_images/fc13338d-94af-4aa9-99da-e14d17f0868c/Sunset-scaled.jpg?width=1000&amp;format=webp" alt="Horseback riding" class="w-40 h-64 rounded-lg object-cover object-center">
													<p class="text-hh-base text-hh-on-base text-">Horseback riding</p>
												</div>
											</a>
										</div>
									</div>
								</div>
								<!-- End Recommendations -->
								<!-- Start Amenities -->
								<div class="flex flex-col">
									<div class="flex flex-row justify-between">
										<div>
											<p class="text-lg font-semibold text-hh-on-base leading-normal tracking-wider">
												Amenities
											</p>
										</div>
										<div>
											<p class="text-sm font-semibold text-hh-on-base leading-normal tracking-wide">
												<a href="" aria-label="View all amenities">View all</a>
											</p>
										</div>
									</div>
									<div class="flex gap-4 flex-nowrap mt-2 overflow-x-auto no-scrollbar snap-x">
										<div class="flex-none snap-start">
											<a href="">
												<div class="w-32 h-auto aspect-square flex flex-col gap-2">
													<div class="w-32 h-auto aspect-square bg-hh-base90 rounded-md flex items-center">
														<div class="rounded-full w-24 h-24 bg-hh-base mx-auto flex items-center">
															<svg width="40" height="40" viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg" class="mx-auto">
																<path d="M37 10.1628V7C37 4.79086 35.2091 3 33 3V3C30.7909 3 29 4.79086 29 7V31" stroke="#ffffff" stroke-width="1.2" stroke-linecap="round"></path>
																<path d="M19 10.1628V7C19 4.79086 17.2091 3 15 3V3C12.7909 3 11 4.79086 11 7V31" stroke="#ffffff" stroke-width="1.2" stroke-linecap="round"></path>
																<line x1="11" y1="16.4" x2="29" y2="16.4" stroke="#ffffff" stroke-width="1.2"></line>
																<line x1="11" y1="24.4" x2="29" y2="24.4" stroke="#ffffff" stroke-width="1.2"></line>
																<path d="M1 33L4.94419 30.7165C6.74483 29.674 8.99214 29.798 10.6672 31.0323V31.0323C12.2974 32.2335 14.4745 32.3857 16.256 31.4231L17.8744 30.5486C19.6239 29.6032 21.7618 29.7527 23.3627 30.9323V30.9323C25.0568 32.1806 27.341 32.2692 29.1267 31.1558L29.5126 30.9152C31.3927 29.743 33.7761 29.743 35.6563 30.9152L39 33" stroke="#ffffff" stroke-width="1.2" stroke-linecap="round"></path>
																<path d="M1 39L4.94419 36.7165C6.74483 35.674 8.99214 35.798 10.6672 37.0323V37.0323C12.2974 38.2335 14.4745 38.3857 16.256 37.4231L17.8744 36.5486C19.6239 35.6032 21.7618 35.7527 23.3627 36.9323V36.9323C25.0568 38.1806 27.341 38.2692 29.1267 37.1558L29.5126 36.9152C31.3927 35.743 33.7761 35.743 35.6563 36.9152L39 39" stroke="#ffffff" stroke-width="1.2" stroke-linecap="round"></path>
															</svg>
														</div>
													</div>
													<p class="text-sm text-hh-on-base line-clamp-2">Pool</p>
												</div>
											</a>
										</div>
										<div class="flex-none snap-start">
											<a href="">
												<div class="w-32 h-auto aspect-square flex flex-col gap-2">
													<div class="w-32 h-auto aspect-square bg-hh-base90 rounded-md flex items-center">
														<div class="rounded-full w-24 h-24 bg-hh-base mx-auto flex items-center">
															<svg width="40" height="40" viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg" class="mx-auto">
																<path fill-rule="evenodd" clip-rule="evenodd" d="M32.3174 37.253L36.9841 23.253C37.1568 22.735 36.7712 22.2 36.2251 22.2H28.6396C27.1142 22.2 25.8009 21.1233 25.5017 19.6276L25.4664 19.4509C25.2047 18.1421 24.0555 17.2 22.7208 17.2H17.2792C15.9445 17.2 14.7953 18.1421 14.5336 19.4509L14.4982 19.6276C14.1991 21.1233 12.8858 22.2 11.3604 22.2H3.77485C3.2288 22.2 2.84323 22.735 3.0159 23.253L7.68257 37.253C7.79146 37.5797 8.09717 37.8 8.44152 37.8H31.5585C31.9028 37.8 32.2085 37.5797 32.3174 37.253ZM3.77485 21C2.40973 21 1.44579 22.3374 1.87748 23.6325L6.54415 37.6325C6.81638 38.4491 7.58066 39 8.44152 39H31.5585C32.4193 39 33.1836 38.4491 33.4558 37.6325L38.1225 23.6325C38.5542 22.3374 37.5903 21 36.2251 21H28.6396C27.6862 21 26.8654 20.3271 26.6784 19.3922L26.6431 19.2155C26.2692 17.3458 24.6275 16 22.7208 16H17.2792C15.3725 16 13.7308 17.3458 13.3569 19.2155L13.3216 19.3922C13.1346 20.3271 12.3138 21 11.3604 21H3.77485Z" stroke="#ffffff" stroke-width="1.2"></path>
																<path fill-rule="evenodd" clip-rule="evenodd" d="M22 20H18C17.4477 20 17 20.4477 17 21C17 21.5523 17.4477 22 18 22H22C22.5523 22 23 21.5523 23 21C23 20.4477 22.5523 20 22 20ZM18 19C16.8954 19 16 19.8954 16 21C16 22.1046 16.8954 23 18 23H22C23.1046 23 24 22.1046 24 21C24 19.8954 23.1046 19 22 19H18Z" stroke="#ffffff" stroke-width="1.2"></path>
																<path fill-rule="evenodd" clip-rule="evenodd" d="M3.5 15C3.5 13.6193 4.61929 12.5 6 12.5H34.0604C35.638 12.5 36.8212 13.9433 36.5118 15.4903L36.0141 17.9792L36.9808 21.3626L36.0192 21.6374L35.1228 18.5H25.5V17.5H35.0901L35.5313 15.2942C35.7169 14.366 35.007 13.5 34.0604 13.5H6C5.17157 13.5 4.5 14.1716 4.5 15V21.5H3.5V15ZM14.5 18.5H8.5V17.5H14.5V18.5Z" stroke="#ffffff" stroke-width="1.2"></path>
																<path fill-rule="evenodd" clip-rule="evenodd" d="M33 3.5C33.8284 3.5 34.5 4.17157 34.5 5V11C34.5 11.8284 33.8284 12.5 33 12.5H4.30997C3.53935 12.5 2.8941 11.9161 2.81742 11.1493L2.71742 10.1493C2.62912 9.26623 3.32254 8.5 4.20998 8.5H30.5V7.5H4.5C3.67157 7.5 3 6.82843 3 6V5C3 4.17157 3.67157 3.5 4.5 3.5H33ZM2.86544 7.89167C2.33538 7.43325 2 6.75579 2 6V5C2 3.61929 3.11929 2.5 4.5 2.5H33C34.3807 2.5 35.5 3.61929 35.5 5V11C35.5 12.3807 34.3807 13.5 33 13.5H4.30997C3.0256 13.5 1.95018 12.5268 1.82238 11.2488L1.72238 10.2488C1.62467 9.27168 2.10124 8.3804 2.86544 7.89167Z" stroke="#ffffff" stroke-width="1.2"></path>
																<path fill-rule="evenodd" clip-rule="evenodd" d="M6.3419 25.0257C6.60387 24.9383 6.88703 25.0799 6.97436 25.3419L9.97436 34.3419C10.0617 34.6039 9.9201 34.887 9.65813 34.9744C9.39616 35.0617 9.113 34.9201 9.02567 34.6581L6.02567 25.6581C5.93835 25.3962 6.07993 25.113 6.3419 25.0257Z" stroke="#ffffff" stroke-width="1.2"></path>
															</svg>
														</div>
													</div>
													<p class="text-sm text-hh-on-base line-clamp-2">Laundry Services</p>
												</div>
											</a>
										</div>
										<div class="flex-none snap-start">
											<a href="">
												<div class="w-32 h-auto aspect-square flex flex-col gap-2">
													<div class="w-32 h-auto aspect-square bg-hh-base90 rounded-md flex items-center">
														<div class="rounded-full w-24 h-24 bg-hh-base mx-auto flex items-center">
															<svg width="40" height="40" viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg" class="mx-auto">
																<path fill-rule="evenodd" clip-rule="evenodd" d="M11.87 4.57634C11.2205 4.57634 10.6563 5.02302 10.5073 5.65518L7.38669 18.8958C7.32751 19.147 7.51802 19.3876 7.77602 19.3876H10.7226C10.9128 19.3876 11.0766 19.2538 11.1146 19.0675L13.2181 8.74751C13.2842 8.42282 13.6011 8.21325 13.9258 8.27943C14.2505 8.34561 14.4601 8.66248 14.3939 8.98718L12.2904 19.3071C12.1385 20.0523 11.4831 20.5876 10.7226 20.5876H7.77602C6.74402 20.5876 5.98195 19.625 6.21869 18.6206L9.33932 5.3799C9.61602 4.20589 10.6638 3.37634 11.87 3.37634H14.8035C15.1349 3.37634 15.4035 3.64497 15.4035 3.97634C15.4035 4.30771 15.1349 4.57634 14.8035 4.57634H11.87ZM26.3947 3.97634C26.3947 3.64497 26.6633 3.37634 26.9947 3.37634H28.4199C29.6152 3.37634 30.6565 4.19132 30.9437 5.35161L34.2239 18.6031C34.4737 19.6121 33.7102 20.5876 32.6708 20.5876H29.993C29.2277 20.5876 28.5696 20.0457 28.4227 19.2947L26.4059 8.98251C26.3422 8.6573 26.5543 8.34211 26.8795 8.2785C27.2047 8.2149 27.5199 8.42697 27.5835 8.75218L29.6004 19.0644C29.6372 19.2521 29.8017 19.3876 29.993 19.3876H32.6708C32.9307 19.3876 33.1215 19.1437 33.0591 18.8915L29.7789 5.63995C29.6242 5.01518 29.0635 4.57634 28.4199 4.57634H26.9947C26.6633 4.57634 26.3947 4.30771 26.3947 3.97634Z" stroke="#ffffff" stroke-width="1.2"></path>
																<path fill-rule="evenodd" clip-rule="evenodd" d="M6.83189 16.7585C6.83191 16.4272 7.10056 16.1585 7.43193 16.1586H11.9914C12.3228 16.1586 12.5914 16.4272 12.5914 16.7586C12.5914 17.0899 12.3228 17.3586 11.9914 17.3586H7.43184C7.10047 17.3585 6.83186 17.0899 6.83189 16.7585ZM28.0529 17.0815C28.0529 16.7501 28.3216 16.4815 28.6529 16.4815H32.5277C32.8591 16.4815 33.1277 16.7501 33.1277 17.0815C33.1277 17.4129 32.8591 17.6815 32.5277 17.6815H28.6529C28.3216 17.6815 28.0529 17.4129 28.0529 17.0815Z" stroke="#ffffff" stroke-width="1.2"></path>
																<path fill-rule="evenodd" clip-rule="evenodd" d="M27.1754 7.99694C27.5059 8.0208 27.7545 8.30806 27.7307 8.63857L26.7825 21.7774L27.67 37.1188C27.7232 38.0373 26.9927 38.8112 26.0727 38.8112H13.5463C12.6106 38.8112 11.8746 38.0119 11.9517 37.0795L13.2187 21.7484V8.59539C13.2187 8.26402 13.4873 7.99539 13.8187 7.99539C14.1501 7.99539 14.4187 8.26402 14.4187 8.59539V21.7979L13.1476 37.1783C13.1284 37.4114 13.3123 37.6112 13.5463 37.6112H26.0727C26.3027 37.6112 26.4853 37.4177 26.472 37.1881L25.58 21.7688L26.5338 8.5522C26.5576 8.22169 26.8449 7.97309 27.1754 7.99694Z" stroke="#ffffff" stroke-width="1.2"></path>
																<path fill-rule="evenodd" clip-rule="evenodd" d="M12.1944 35.1422C12.1944 34.8109 12.4631 34.5422 12.7944 34.5422H26.7981C27.1295 34.5422 27.3981 34.8109 27.3981 35.1422C27.3981 35.4736 27.1295 35.7422 26.7981 35.7422H12.7944C12.4631 35.7422 12.1944 35.4736 12.1944 35.1422Z" stroke="#ffffff" stroke-width="1.2"></path>
																<path fill-rule="evenodd" clip-rule="evenodd" d="M13.4903 19.3277C13.4903 18.9963 13.759 18.7277 14.0903 18.7277H15.9972C16.3285 18.7277 16.5972 18.9963 16.5972 19.3277C16.5972 19.659 16.3285 19.9277 15.9972 19.9277H14.0903C13.759 19.9277 13.4903 19.659 13.4903 19.3277ZM18.2516 19.3277C18.2516 18.9963 18.5202 18.7277 18.8516 18.7277H26.1812C26.5125 18.7277 26.7812 18.9963 26.7812 19.3277C26.7812 19.659 26.5125 19.9277 26.1812 19.9277H18.8516C18.5202 19.9277 18.2516 19.659 18.2516 19.3277ZM13.4903 22.2288C13.4903 21.8974 13.759 21.6288 14.0903 21.6288H15.9972C16.3285 21.6288 16.5972 21.8974 16.5972 22.2288C16.5972 22.5602 16.3285 22.8288 15.9972 22.8288H14.0903C13.759 22.8288 13.4903 22.5602 13.4903 22.2288ZM18.2516 22.2288C18.2516 21.8974 18.5202 21.6288 18.8516 21.6288H26.1812C26.5125 21.6288 26.7812 21.8974 26.7812 22.2288C26.7812 22.5602 26.5125 22.8288 26.1812 22.8288H18.8516C18.5202 22.8288 18.2516 22.5602 18.2516 22.2288Z" stroke="#ffffff" stroke-width="1.2"></path>
																<path fill-rule="evenodd" clip-rule="evenodd" d="M16.6136 18.5804V28.4978H18.0036V18.5804H16.6136ZM16.4136 17.3804C15.8613 17.3804 15.4136 17.8281 15.4136 18.3804V28.6978C15.4136 29.25 15.8613 29.6978 16.4136 29.6978H18.2036C18.7559 29.6978 19.2036 29.25 19.2036 28.6978V18.3804C19.2036 17.8281 18.7559 17.3804 18.2036 17.3804H16.4136Z" stroke="#ffffff" stroke-width="1.2"></path>
																<path fill-rule="evenodd" clip-rule="evenodd" d="M16.1428 2.38896C15.9773 2.38896 15.8289 2.49091 15.7695 2.6454L15.7379 2.7274C15.4908 3.36993 15.5316 4.08762 15.8497 4.69808L20.0023 12.6654L25.3331 5.20096C25.772 4.58626 25.896 3.80077 25.6677 3.08074L25.5369 2.66806C25.4842 2.50188 25.3299 2.38896 25.1556 2.38896H16.1428ZM20.6245 13.859L26.3096 5.89836C26.9681 4.97631 27.1541 3.79807 26.8116 2.71803L26.6807 2.30536C26.47 1.64062 25.8529 1.18896 25.1556 1.18896H16.1428C15.4807 1.18896 14.887 1.59673 14.6494 2.21469L14.6179 2.2967C14.2473 3.26049 14.3083 4.33703 14.7856 5.25271L22.099 19.2845C22.2522 19.5784 22.6146 19.6924 22.9084 19.5393C23.2023 19.3861 23.3163 19.0237 23.1632 18.7299L20.6245 13.859Z" stroke="#ffffff" stroke-width="1.2"></path>
																<path fill-rule="evenodd" clip-rule="evenodd" d="M23.9507 3.55031C24.2202 3.74312 24.2823 4.11789 24.0895 4.38739L19.0353 11.4518C18.8425 11.7213 18.4677 11.7835 18.1982 11.5907C17.9287 11.3979 17.8666 11.0231 18.0594 10.7536L23.1136 3.68916C23.3064 3.41966 23.6812 3.35749 23.9507 3.55031Z" stroke="#ffffff" stroke-width="1.2"></path>
																<path fill-rule="evenodd" clip-rule="evenodd" d="M18.5035 4.62603H23.5309C23.8623 4.62603 24.1309 4.3574 24.1309 4.02603C24.1309 3.69465 23.8623 3.42603 23.5309 3.42603H17.8346C17.2297 3.42603 16.8436 4.07157 17.1299 4.60453L19.5693 9.1468C19.726 9.43874 20.0898 9.5483 20.3817 9.39152C20.6737 9.23474 20.7832 8.87098 20.6265 8.57904L18.5035 4.62603Z" stroke="#ffffff" stroke-width="1.2"></path>
															</svg>
														</div>
													</div>
													<p class="text-sm text-hh-on-base line-clamp-2">Bathrobes</p>
												</div>
											</a>
										</div>
										<div class="flex-none snap-start">
											<a href="">
												<div class="w-32 h-auto aspect-square flex flex-col gap-2">
													<div class="w-32 h-auto aspect-square bg-hh-base90 rounded-md flex items-center">
														<div class="rounded-full w-24 h-24 bg-hh-base mx-auto flex items-center">
															<svg width="40" height="40" viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg" class="mx-auto">
																<g clip-path="url(#clip0_536_19882)">
																	<path d="M33 8.71633C33.375 7.36316 34.5 6.46097 35.625 7.36317C36.5075 8.07091 37.5 10.0695 39 8.26526" stroke="#ffffff" stroke-width="1.2" stroke-linecap="round"></path>
																	<path d="M33 13.7163C33.375 12.3632 34.5 11.461 35.625 12.3632C36.5075 13.0709 37.5 15.0695 39 13.2653" stroke="#ffffff" stroke-width="1.2" stroke-linecap="round"></path>
																	<path d="M29.3999 11C29.3999 11.3429 29.3959 11.7757 29.3915 12.2432C29.3824 13.2277 29.3719 14.3663 29.3943 15.1441C29.3205 15.2055 29.2035 15.2883 29.0343 15.3914C28.6416 15.6309 28.0547 15.9281 27.3117 16.2643C25.8313 16.9344 23.7951 17.731 21.608 18.4962C19.4219 19.2609 17.0969 19.9901 15.04 20.5273C12.9646 21.0693 11.2196 21.4 10.1662 21.4C4.92658 21.4 0.6 16.7892 0.6 11C0.6 5.21083 4.92658 0.6 10.1662 0.6C11.2195 0.6 12.9617 0.930672 15.0338 1.47266C17.0872 2.00979 19.4083 2.73897 21.5917 3.50377C23.7761 4.26891 25.8111 5.06562 27.2939 5.73581C28.0379 6.07209 28.6273 6.36956 29.0236 6.60953C29.2018 6.71742 29.3241 6.80368 29.3999 6.86709V6.86771V6.87469V6.88168V6.88869V6.89572V6.90277V6.90984V6.91693V6.92404V6.93117V6.93832V6.94548V6.95267V6.95987V6.96709V6.97433V6.98159V6.98887V6.99616V7.00347V7.0108V7.01815V7.02552V7.03291V7.04031V7.04773V7.05517V7.06262V7.0701V7.07759V7.08509V7.09262V7.10016V7.10772V7.1153V7.12289V7.1305V7.13813V7.14577V7.15343V7.16111V7.1688V7.17651V7.18423V7.19197V7.19973V7.2075V7.21529V7.2231V7.23092V7.23875V7.2466V7.25447V7.26235V7.27025V7.27816V7.28609V7.29404V7.30199V7.30997V7.31796V7.32596V7.33397V7.34201V7.35005V7.35811V7.36619V7.37428V7.38238V7.3905V7.39863V7.40677V7.41493V7.42311V7.43129V7.43949V7.44771V7.45593V7.46417V7.47243V7.48069V7.48897V7.49726V7.50557V7.51389V7.52222V7.53056V7.53892V7.54729V7.55567V7.56406V7.57247V7.58088V7.58931V7.59776V7.60621V7.61468V7.62315V7.63164V7.64014V7.64865V7.65718V7.66571V7.67426V7.68281V7.69138V7.69996V7.70855V7.71715V7.72576V7.73439V7.74302V7.75166V7.76032V7.76898V7.77766V7.78634V7.79503V7.80374V7.81245V7.82118V7.82991V7.83866V7.84741V7.85617V7.86494V7.87373V7.88252V7.89132V7.90013V7.90895V7.91777V7.92661V7.93545V7.94431V7.95317V7.96204V7.97092V7.9798V7.9887V7.9976V8.00652V8.01544V8.02436V8.0333V8.04224V8.05119V8.06015V8.06912V8.07809V8.08707V8.09606V8.10506V8.11406V8.12307V8.13209V8.14111V8.15014V8.15918V8.16822V8.17727V8.18633V8.19539V8.20446V8.21353V8.22261V8.2317V8.2408V8.24989V8.259V8.26811V8.27723V8.28635V8.29548V8.30461V8.31375V8.32289V8.33204V8.34119V8.35035V8.35951V8.36868V8.37785V8.38703V8.39621V8.4054V8.41459V8.42378V8.43298V8.44219V8.45139V8.4606V8.46982V8.47904V8.48826V8.49749V8.50672V8.51595V8.52519V8.53443V8.54367V8.55292V8.56217V8.57142V8.58067V8.58993V8.59919V8.60846V8.61772V8.62699V8.63626V8.64553V8.65481V8.66409V8.67337V8.68265V8.69193V8.70122V8.7105V8.71979V8.72908V8.73837V8.74767V8.75696V8.76626V8.77555V8.78485V8.79415V8.80345V8.81275V8.82205V8.83135V8.84066V8.84996V8.85926V8.86857V8.87787V8.88717V8.89648V8.90578V8.91508V8.92439V8.93369V8.943V8.9523V8.9616V8.9709V8.9802V8.9895V8.9988V9.0081V9.0174V9.0267V9.03599V9.04529V9.05458V9.06387V9.07316V9.08245V9.09173V9.10102V9.1103V9.11958V9.12886V9.13814V9.14741V9.15669V9.16596V9.17522V9.18449V9.19375V9.20301V9.21227V9.22152V9.23078V9.24002V9.24927V9.25851V9.26775V9.27699V9.28622V9.29545V9.30467V9.3139V9.32311V9.33233V9.34154V9.35074V9.35995V9.36914V9.37834V9.38753V9.39671V9.40589V9.41507V9.42424V9.43341V9.44257V9.45173V9.46088V9.47003V9.47917V9.48831V9.49744V9.50656V9.51568V9.5248V9.53391V9.54301V9.55211V9.5612V9.57029V9.57937V9.58844V9.59751V9.60657V9.61562V9.62467V9.63371V9.64275V9.65178V9.6608V9.66981V9.67882V9.68782V9.69682V9.7058V9.71478V9.72375V9.73272V9.74168V9.75062V9.75957V9.7685V9.77743V9.78634V9.79525V9.80416V9.81305V9.82193V9.83081V9.83968V9.84854V9.85739V9.86623V9.87507V9.88389V9.89271V9.90152V9.91031V9.9191V9.92788V9.93665V9.94541V9.95416V9.9629V9.97164V9.98036V9.98907V9.99777V10.0065V10.0151V10.0238V10.0325V10.0411V10.0498V10.0584V10.067V10.0756V10.0842V10.0928V10.1014V10.11V10.1185V10.1271V10.1356V10.1441V10.1526V10.1611V10.1696V10.1781V10.1865V10.195V10.2034V10.2119V10.2203V10.2287V10.2371V10.2454V10.2538V10.2622V10.2705V10.2788V10.2871V10.2954V10.3037V10.312V10.3203V10.3285V10.3368V10.345V10.3532V10.3614V10.3696V10.3777V10.3859V10.394V10.4022V10.4103V10.4184V10.4265V10.4345V10.4426V10.4506V10.4587V10.4667V10.4747V10.4827V10.4906V10.4986V10.5065V10.5145V10.5224V10.5303V10.5381V10.546V10.5538V10.5617V10.5695V10.5773V10.5851V10.5928V10.6006V10.6083V10.6161V10.6238V10.6315V10.6391V10.6468V10.6544V10.662V10.6696V10.6772V10.6848V10.6924V10.6999V10.7074V10.7149V10.7224V10.7299V10.7373V10.7448V10.7522V10.7596V10.767V10.7743V10.7817V10.789V10.7963V10.8036V10.8109V10.8181V10.8254V10.8326V10.8398V10.847V10.8541V10.8613V10.8684V10.8755V10.8826V10.8896V10.8967V10.9037V10.9107V10.9177V10.9247V10.9316V10.9385V10.9455V10.9523V10.9592V10.9661V10.9729V10.9797V10.9865V10.9933V11Z" stroke="#ffffff" stroke-width="1.2"></path>
																	<path d="M11.3209 36.4732L7.40216 21.0525L14.0429 21.0525L17.817 34.7533C18.3168 36.5677 17.2291 38.4387 15.4051 38.9023C13.6066 39.3593 11.778 38.2718 11.3209 36.4732Z" stroke="#ffffff" stroke-width="1.2"></path>
																	<circle cx="11" cy="11" r="5.4" stroke="#ffffff" stroke-width="1.2"></circle>
																	<path d="M25 5L25 17" stroke="#ffffff" stroke-width="1.2"></path>
																</g>
																<defs>
																	<clipPath id="clip0_536_19882">
																		<rect width="40" height="40" fill="#ffffff"></rect>
																	</clipPath>
																</defs>
															</svg>
														</div>
													</div>
													<p class="text-sm text-hh-on-base line-clamp-2">Hair Dryer</p>
												</div>
											</a>
										</div>
										<div class="flex-none snap-start">
											<a href="">
												<div class="w-32 h-auto aspect-square flex flex-col gap-2">
													<div class="w-32 h-auto aspect-square bg-hh-base90 rounded-md flex items-center">
														<div class="rounded-full w-24 h-24 bg-hh-base mx-auto flex items-center">
															<svg width="40" height="40" viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg" class="mx-auto">
																<circle cx="20" cy="31" r="2" fill="#ffffff"></circle>
																<path d="M2.5 12.8826C7.17869 9.19814 13.0826 7 19.5 7C25.9174 7 31.8213 9.19814 36.5 12.8826" stroke="#ffffff" stroke-width="1.2" stroke-linecap="round"></path>
																<path d="M7.5 19.6906C10.8409 16.7697 15.2138 15 20 15C24.551 15 28.7283 16.6001 32 19.2683" stroke="#ffffff" stroke-width="1.2" stroke-linecap="round"></path>
																<path d="M12 25.4501C14.0055 23.3258 16.8479 22 20 22C23.1521 22 25.9945 23.3258 28 25.4501" stroke="#ffffff" stroke-width="1.2" stroke-linecap="round"></path>
															</svg>
														</div>
													</div>
													<p class="text-sm text-hh-on-base line-clamp-2">WiFI</p>
												</div>
											</a>
										</div>
									</div>
								</div>
								<!-- End Amenities -->
								<!-- Start of Guidebooks -->
								<div class="flex flex-col">
									<div class="flex flex-row justify-between">
										<div>
											<p class="text-lg font-semibold text-hh-on-base leading-normal tracking-wider">
												Guidebooks
											</p>
										</div>
									</div>
									<div class="flex flex-col mt-2 overflow-x-auto no-scrollbar snap-x divide-y divide-hh-base80">
										<div class="flex-none snap-start text-hh-on-base py-4 font-medium">
											<a href="">
												<div class="flex flex-row justify-between pr-4 line-clamp-1">
													<div class="text-hh-on-base text-hh-base font-medium leading-tight">
														Punta Cana Q&amp;A
													</div>
													<div class="flex-none">
														<svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="fill-hh-on-base">
															<path d="M20.6919 12.2869C20.6539 12.3789 20.599 12.4618 20.53 12.5308L16.53 16.5308C16.384 16.6768 16.192 16.7508 16 16.7508C15.808 16.7508 15.616 16.6778 15.47 16.5308C15.177 16.2378 15.177 15.7628 15.47 15.4698L18.1899 12.7498H4C3.586 12.7498 3.25 12.4138 3.25 11.9998C3.25 11.5858 3.586 11.2498 4 11.2498H18.189L15.469 8.52981C15.176 8.23681 15.176 7.76177 15.469 7.46877C15.762 7.17577 16.237 7.17577 16.53 7.46877L20.53 11.4688C20.599 11.5378 20.6539 11.6207 20.6919 11.7127C20.7679 11.8967 20.7679 12.1029 20.6919 12.2869Z"></path>
														</svg>
													</div>
												</div>
											</a>
										</div>
										<div class="flex-none snap-start text-hh-on-base py-4 font-medium">
											<a href="">
												<div class="flex flex-row justify-between pr-4 line-clamp-1">
													<div class="text-hh-on-base text-hh-base font-medium leading-tight">
														Best things to do in Punta Cana
													</div>
													<div class="flex-none">
														<svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="fill-hh-on-base">
															<path d="M20.6919 12.2869C20.6539 12.3789 20.599 12.4618 20.53 12.5308L16.53 16.5308C16.384 16.6768 16.192 16.7508 16 16.7508C15.808 16.7508 15.616 16.6778 15.47 16.5308C15.177 16.2378 15.177 15.7628 15.47 15.4698L18.1899 12.7498H4C3.586 12.7498 3.25 12.4138 3.25 11.9998C3.25 11.5858 3.586 11.2498 4 11.2498H18.189L15.469 8.52981C15.176 8.23681 15.176 7.76177 15.469 7.46877C15.762 7.17577 16.237 7.17577 16.53 7.46877L20.53 11.4688C20.599 11.5378 20.6539 11.6207 20.6919 11.7127C20.7679 11.8967 20.7679 12.1029 20.6919 12.2869Z"></path>
														</svg>
													</div>
												</div>
											</a>
										</div>
									</div>
								</div>
								<!-- End of Guidebooks -->
								<!-- Start 'My Party' -->
								<div class="flex flex-col gap-4 inline-block">
									<div class="flex flex-row justify-between">
										<div>
											<p class="text-lg font-medium text-hh-on-base">
												De hosts:
											</p>
										</div>
									</div>
									<div class="flex flex-row gap-4 mt-2 overflow-x-auto no-scrollbar snap-x">
										<div class="flex-none snap-start">
											<div class="flex flex-col gap-2 w-20">
												<img src="~/assets/Verena.webp" alt="Sjeel Koster" class="w-20 h-20 rounded-full">
												<p class="text-sm text-hh-on-base text-center line-clamp-2">
													Verena
												</p>
											</div>
										</div>
										<div class="flex-none snap-start">
											<div class="flex flex-col gap-2 w-20">
												<div class="w-20 h-20 bg-hh-base90 rounded-full flex items-center text-center">
													<svg width="30" height="30" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg" class="mx-auto">
														<path d="M15.0113 13.4375C12.0813 13.4375 9.69879 11.0538 9.69879 8.125C9.69879 5.19625 12.0813 2.8125 15.0113 2.8125C17.9413 2.8125 20.3238 5.19625 20.3238 8.125C20.3238 11.0538 17.9413 13.4375 15.0113 13.4375ZM15.0113 4.6875C13.115 4.6875 11.5738 6.22875 11.5738 8.125C11.5738 10.0212 13.115 11.5625 15.0113 11.5625C16.9075 11.5625 18.4488 10.0212 18.4488 8.125C18.4488 6.22875 16.9063 4.6875 15.0113 4.6875ZM19.9962 27.1875H10.0038C6.97881 27.1875 5.3125 25.5313 5.3125 22.5238C5.3125 19.1976 7.195 15.3125 12.5 15.3125H17.5C22.805 15.3125 24.6875 19.1963 24.6875 22.5238C24.6875 25.5313 23.0212 27.1875 19.9962 27.1875ZM12.5 17.1875C7.57125 17.1875 7.1875 21.2713 7.1875 22.5238C7.1875 24.4788 8.03006 25.3125 10.0038 25.3125H19.9962C21.9699 25.3125 22.8125 24.4788 22.8125 22.5238C22.8125 21.2726 22.4288 17.1875 17.5 17.1875H12.5Z" fill="#ffffff"></path>
													</svg>
												</div>
												<p class="text-sm text-hh-on-base text-center line-clamp-2">
													Olaf
												</p>
											</div>
										</div>
									</div>
								</div>
								<!-- End 'My Party' -->
							</div>
							<!--- End Main Content -->
						</div>
					</div>
                </div>

            </div>
		</main>
</template>

<script setup>

const { data: home } = reactive(await useAsyncData("home", () =>
	queryContent("/pages/home").findOne())
);

setSeoHead(home.SEOmetaData);

</script>

<style scoped>

</style>
