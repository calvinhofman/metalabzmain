<script setup lang="ts">



</script>

<template>
  <div className="">
    <div v-if="isOpen" class="fixed inset-0 flex items-center justify-center z-[20]">
      <div class="bg-gray-800 bg-opacity-50 z-10 absolute inset-0"></div>
      <div class="bg-[#A3A4EF] rounded-lg p-6 z-40">
        <div class="flex flex-row justify-between items-center mb-4">
          <h1 class="text-2xl font-bold">IMPORTANT NOTICE!</h1>
          <button class="z-90 text-white font-bold py-2 px-4" @click="closeModal">
            X
          </button>
        </div>
        <p>MetaBUSD will pause trading 14,July 2023 <br /> in order to migrate to a new token MetaLabz -MLZ</p>
      </div>
    </div>
    <div
      :class="isActive ? 'absolute w-full h-full bg-[#7CCCEC] z-20 p-8 invisible' : 'absolute w-full h-full bg-[#7CCCEC] z-20 p-8'"
      id="navbar">
      <nav class="flex flex-row justify-between items-center">
        <div>
          <p class="font-semibold text-white">
            $MLZ
          </p>
        </div>
        <div class="flex flex-row items-center w-full sm:w-4/12 justify-between">
          <p class="text-white">Find us</p>
          <a href="https://twitter.com/MetaBusdCoin"><img class="w-4 h-4"
              src="../components/images/Icon awesome-twitter-white.png" alt="" /></a>
          <a href="https://www.reddit.com/r/MetaBUSDCoin/"><img class="w-4 h-4"
              src="../components/images/Icon awesome-reddit-alien-white.png" alt="" /></a>
          <a href="https://t.me/+U8iy18bIQdk0M2Zh"><img class="w-4 h-4"
              src="../components/images/Icon awesome-telegram-plane-white.png" alt="" /></a>
          <a href="https://discord.com/invite/r2YU2nPnHj"><img class="w-4 h-4"
              src="../components/images/Icon simple-discord-white.png" alt="" /></a>
          <div><button @click="handleClick"><img class="w-8 h-8" src="../components/images/arrowdown.png" alt=""
                srcset="" /></button></div>
        </div>
      </nav>
      <div class="flex flex-col lg:flex-row justify-between 2xl:px-96 2xl:mt-72">
        <div class="mx-auto">
          <img class="w-12/12" src="../components/images/navbarmouse.png" alt="" />
        </div>
        <div class="flex flex-row items-center space-x-8 mx-auto">
          <div class="flex flex-col text-2xl sm:text-4xl text-white font-bold">
            <div><button @click="navbarLinking" id="aboutnavbar">About</button></div>
            <div><button @click="navbarLinking" id="setusNavbar">Set us apart</button></div>
            <div><button @click="navbarLinking" id="roadmapNavbar">Roadmap</button></div>
            <div><button @click="navbarLinking" id="teamNavbar">Team</button></div>
            <div><button @click="navbarLinking" id="partnerNavbar">Partners</button></div>
            <div><button @click="navbarLinking" id="buyNavbar">Buy online</button></div>
            <div><button @click="navbarLinking" id="contactNavbar">Contact</button></div>
          </div>
          <div class="flex flex-col text-2xl sm:text-4xl text-white font-bold">
            <div><RouterLink to="/staking">staking</RouterLink></div>
            <div><a href="https://liquidlabz.com/">Farming</a></div>
            <div><a href="https://nftlabz.app/">Nfts</a></div>
            <!--
          <div><a href="http://">Rewards</a></div>
          <div><a href="http://">Staking</a></div>
          <div><a href="http://">Nfts</a></div>
          -->
          </div>
        </div>
        <div class="mx-auto">
          <img class="w-32 sm:w-full" src="../components/images/rocketnavbar.png" alt="" />
        </div>
      </div>
    </div>
    <header className="w-full p-8  pb-0">
      <nav className="flex sm:flex-row flex-col-reverse justify-between items-center ">
        <div>
          <p className="font-semibold">
            $MLZ
          </p>
        </div>
        <div className="flex flex-row items-center">
          <img className="w-28 h-16" src="../components/images/logo.png" alt="" srcset="" />
        </div>
        <div className="flex flex-row items-center sm:w-3/12 w-full justify-between">
          <p>Find us</p>
          <a href="https://twitter.com/MetaBusdCoin"><img className="w-4 h-4"
              src="../components/images/Icon awesome-twitter.png" alt="" /></a>
          <a href="https://www.reddit.com/r/MetaBUSDCoin/"><img className="w-4 h-4"
              src="../components/images/Icon awesome-reddit-alien.png" alt="" /></a>
          <a href="https://t.me/+U8iy18bIQdk0M2Zh"><img className="w-4 h-4"
              src="../components/images/Icon awesome-telegram-plane.png" alt="" /></a>
          <a href="https://discord.com/invite/r2YU2nPnHj"><img className="w-4 h-4"
              src="../components/images/Icon simple-discord.png" alt="" /></a>
          <div><button @click="handleClick(!isActive)"><img className="w-8 h-4" src="../components/images/navbar.png"
                alt="" srcset="" /></button></div>
        </div>
      </nav>
      <div className="mt-32" id="about">
        <div className="flex flex-col lg:flex-row justify-center">
          <div className=" lg:w-5/12 ">
            <h1 className="text-2xl">
              Welcome to META LABZ <br />
              <br />
            </h1>
            <p className="sm:w-8/12 w-12/12 text-2xl">
              a leading web3 development firm that specializes in creating
              immersive virtual reality games and experiences, as well as
              cutting-edge smart contracts, NFTs, dapps, and other related
              items.
            </p>
            <div className="right-0 flex justify-end">
              <div className="absolute">
                <div
                  className=" z-0 flex justify-end  mt-20 xl:w-[32rem] lg:w-[90rem] text-center p-8 font-bold text-6xl text-white right-0">
                  <a className="bg-[#A3A4EF] z-0  xl:w-[60rem] lg:w-[28rem] text-center p-8 px-24 font-bold text-2xl sm:text-4xl text-white "
                    href="#buy">
                    BUY NOW
                  </a>
                </div>
              </div>
              <div className="mt-48 z-10">
                <p className="sm:w-8/12 xl:w-10/12 lg:w-[29rem] mb-12 text-white text-xl bg-[#7CCCEC] p-4">
                  Formerly known as MetaBUSDCoin, we have established
                  ourselves as a well-respected and reliable name within the
                  blockchain and cryptocurrency space. At MetaLabz, we are
                  committed to pushing the boundaries of what is possible with
                  web3 technology. Our team of experienced developers and
                  designers has a deep understanding of blockchain technology
                  and a passion for creating innovative solutions that
                  leverage the power of decentralized networks. Whether you
                  are looking to develop a new VR game, launch an NFT
                  marketplace, or build a custom smart contract, we have the
                  expertise and experience to help you achieve your goals.
                </p>
              </div>
            </div>
          </div>
          <div className="xl:w-2/12"></div>
          <div className="lg:w-5/12">
            <img className="w-[60rem] banner-img" src="../components/images/metalabz_side.png" alt="" />
          </div>
        </div>
        <div className="mx-auto sm:w-2/12 w-8/12 ">
          <div className="bg-[#A3A4EF] h-52">
            <img className="mx-auto py-24 banner-img" src="../components/images/Icon ionic-ios-arrow-down.png" alt="" />
          </div>
        </div>
      </div>
    </header>
    <div className="bg-[#A3A4EF] w-full p-8" id="setusapart">
      <h2 className="text-center text-5xl my-6 text-white font-bold">
        Our jobs set us apart
      </h2>
      <div className="flex sm:flex-row flex-col justify-between text-white mx-auto space-y-6 sm:space-y-0">
        <div className="flex sm:flex-row flex-col items-center space-x-4 sm:w-4/12 w-12/12">
          <div>
            <img src="../components/images/Icon awesome-dollar-sign.png" alt="" />
          </div>
          <div className="sm:w-8/12">
            <h3 className="text-3xl font-semibold">Reliable & low cost</h3>
            <p className="text-2xl">
              Having a full time staff of developers affords us an opportunity to bring in incredible rates.
            </p>
          </div>
        </div>
        <div className="flex sm:flex-row flex-col items-center space-x-4  sm:w-4/12">
          <div>
            <img src="../components/images/Icon awesome-shield-alt.png" alt="" />
          </div>
          <div className="sm:w-8/12">
            <h3 className="text-3xl font-semibold">Security</h3>
            <p className="text-2xl">
              MetaLabz is a trusted name in the space due to our extensive development record.

            </p>
          </div>
        </div>
        <div className="flex sm:flex-row flex-col items-center space-x-4  sm:w-4/12">
          <div>
            <img src="../components/images/Icon awesome-exclamation-circle.png" alt="" />
          </div>
          <div className="sm:w-8/12">
            <h3 className="text-3xl font-semibold">Expert support</h3>
            <p className="text-2xl">
              Directly through our website or discord every client inquiry is received and processed 24/7

            </p>
          </div>
        </div>
      </div>
    </div>
    <div className="flex flex-row " id="services">
      <div className="lg:w-4/12 flex flex-col w-0/12 "></div>
      <div className="w-[2.5rem]"></div>
      <div className="lg:w-5/12 w-11/12 p-12">
        <h3 className="font-bold text-2xl sm:text-5xl sm:mt-6">
          Services provided by MetaLabz
        </h3>
        <p className=" sm:w-7/12 lg:px-12 text-[#B5B5B5] sm:text-2xl">
          Press the arrows to cycle between the different services
        </p>
        <div className="flex flex-row justify-between sm:w-8/12 space-y-6 mt-6 ml-12"></div>
        <swiper :modules="modules" :spaceBetween="50" :slidesPerView="1" :loop="true" @slideChange="handleSlideChange"
          @swiper="handleSwiper" :navigation="{ nextEl: '#next', prevEl: '#prev' }">
          <swiper-slide>
            <div class="flex flex-col">
              <div>
                <p class="sm:w-6/12 text-center text-[#7CCCEC] text-4xl font-bold">
                  Smart Contracts
                </p>
                <div class="lg:ml-32">
                  <p class="sm:w-6/12">
                    With years of experience across numerous chains you can feel confident with a great foundation for
                    your ecosystem.
                  </p>
                </div>
                <div class="flex flex-row justify-between w-1/12 mt-4">
                  <button class="text-5xl leading-3" id="prev">‹</button>
                  <button class="text-5xl leading-5" id="next">›</button>
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div className="flex flex-col">
              <div className="">
                <p className="sm:w-6/12 text-center text-[#7CCCEC] text-4xl  font-bold">
                  dApps
                </p>
                <div className="lg:ml-32">
                  <p className="sm:w-6/12 ">
                    Give your customers a robust, secure, and functional
                    access to interact with your smart contracts or easily
                    decipher Blockchain data.
                  </p>
                </div>
                <div className="flex flex-row justify-between w-1/12 mt-4">
                  <button className="text-5xl leading-3" id="prev">
                    ‹
                  </button>
                  <button className="text-5xl leading-5 " id="next">
                    ›
                  </button>
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div className="flex flex-col">
              <div className="">
                <p className="sm:w-6/12 text-center text-[#7CCCEC] text-4xl  font-bold">
                  Websites
                </p>
                <div className="lg:ml-32">
                  <p className="sm:w-6/12 ">
                    Custom professional user friendly websites, including both
                    front-end and back-end development. This is your first
                    impression, you need to make an impact and we can help.
                  </p>
                </div>
                <div className="flex flex-row justify-between w-1/12 mt-4">
                  <button className="text-5xl leading-3" id="prev">
                    ‹
                  </button>
                  <button className="text-5xl leading-5 " id="next">
                    ›
                  </button>
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div className="flex flex-col">
              <div className="">
                <p className="sm:w-6/12 text-center text-[#7CCCEC] text-4xl  font-bold">
                  website design
                </p>
                <div className="lg:ml-32">
                  <p className="sm:w-6/12 ">
                    Strategic website design that captivates users and drives conversions, helping businesses succeed in
                    the digital world.

                  </p>
                </div>
                <div className="flex flex-row justify-between w-1/12 mt-4">
                  <button className="text-5xl leading-3" id="prev">
                    ‹
                  </button>
                  <button className="text-5xl leading-5 " id="next">
                    ›
                  </button>
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div className="flex flex-col">
              <div className="">
                <p className="sm:w-6/12 text-center text-[#7CCCEC] text-4xl  font-bold">
                  Contract Audits
                </p>
                <div className="lg:ml-32">
                  <p className="sm:w-6/12 ">
                    An extra set of eyes always helps when talking about
                    security, we have a multitude of audit solutions for your
                    smart contracts and ecosystem.
                  </p>
                </div>
                <div className="flex flex-row justify-between w-1/12 mt-4">
                  <button className="text-5xl leading-3" id="prev">
                    ‹
                  </button>
                  <button className="text-5xl leading-5 " id="next">
                    ›
                  </button>
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div className="flex flex-col">
              <div className="">
                <p className="sm:w-6/12 text-center text-[#7CCCEC] text-4xl  font-bold">
                  Bots and Scripts
                </p>
                <div className="lg:ml-32">
                  <p className="sm:w-6/12 ">
                    Maybe you need a custom solution for telegram or discord
                    for community engagement. Or an automated solution for an
                    in ecosystem task. Let our team help make this easier for
                    you with our automated solutions.
                  </p>
                </div>
                <div className="flex flex-row justify-between w-1/12 mt-4">
                  <button className="text-5xl leading-3" id="prev">
                    ‹
                  </button>
                  <button className="text-5xl leading-5 " id="next">
                    ›
                  </button>
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div className="flex flex-col">
              <div className="">
                <p className="sm:w-6/12 text-center text-[#7CCCEC] text-4xl  font-bold">
                  Hosting
                </p>
                <div className="lg:ml-32">
                  <p className="sm:w-6/12 ">
                    Keep the important things that you rely upon up and
                    running 24/7 with safe secure performance. Free yourself
                    from the frustration of managing your website,
                    application, or bot hosting.
                  </p>
                </div>
                <div className="flex flex-row justify-between w-1/12 mt-4">
                  <button className="text-5xl leading-3" id="prev">
                    ‹
                  </button>
                  <button className="text-5xl leading-5 " id="next">
                    ›
                  </button>
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div className="flex flex-col">
              <div className="">
                <p className="sm:w-6/12 text-center text-[#7CCCEC] text-4xl  font-bold">
                  Marketing Services

                </p>
                <div className="lg:ml-32">
                  <p className="sm:w-6/12 ">
                    With having assisted in so many launches we have the knowledge needed to find clients success at many
                    budget levels.

                  </p>
                </div>
                <div className="flex flex-row justify-between w-1/12 mt-4">
                  <button className="text-5xl leading-3" id="prev">
                    ‹
                  </button>
                  <button className="text-5xl leading-5 " id="next">
                    ›
                  </button>
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div className="flex flex-col">
              <div className="">
                <p className="sm:w-6/12 text-center text-[#7CCCEC] text-4xl  font-bold">
                  Consulting
                </p>
                <div className="lg:ml-32">
                  <p className="sm:w-6/12 ">
                    Let our experience go to work for your vision. Often times
                    you have the right idea and just need guidance in the
                    proper areas. We have a team dedicated to discovery and
                    analysis that will stick with you until your dream is a
                    reality.
                  </p>
                </div>
                <div className="flex flex-row justify-between w-1/12 mt-4">
                  <button className="text-5xl leading-3" id="prev">
                    ‹
                  </button>
                  <button className="text-5xl leading-5 " id="next">
                    ›
                  </button>
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div className="flex flex-col">
              <div className="">
                <p className="sm:w-6/12 text-center text-[#7CCCEC] text-4xl  font-bold">
                  P2E Games
                </p>
                <div className="lg:ml-32">
                  <p className="sm:w-6/12 ">
                    Drive engagement with revenue-earning games of all genres,
                    complete with features that utilize any and all aspects of
                    your ecosystem.
                  </p>
                </div>
                <div className="flex flex-row justify-between w-1/12 mt-4">
                  <button className="text-5xl leading-3" id="prev">
                    ‹
                  </button>
                  <button className="text-5xl leading-5 " id="next">
                    ›
                  </button>
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div className="flex flex-col">
              <div className="">
                <p className="sm:w-6/12 text-center text-[#7CCCEC] text-4xl  font-bold">
                  VR services
                </p>
                <div className="lg:ml-32">
                  <p className="sm:w-6/12 ">
                    On top of offering gaming services and solutions we also
                    pride ourselves with have an experienced and robust VR/XR
                    development team. Ready for the metaverse?
                  </p>
                </div>
                <div className="flex flex-row justify-between w-1/12 mt-4">
                  <button className="text-5xl leading-3" id="prev">
                    ‹
                  </button>
                  <button className="text-5xl leading-5 " id="next">
                    ›
                  </button>
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div className="flex flex-col">
              <div className="">
                <p className="sm:w-6/12 text-center text-[#7CCCEC] text-4xl  font-bold">
                  Graphic design
                </p>
                <div className="lg:ml-32">
                  <p className="sm:w-6/12 ">
                    Your branding and logo is often what will sell your vision
                    immediately if done right. Let us put our experts to work
                    helping you create an impact.
                  </p>
                </div>
                <div className="flex flex-row justify-between w-1/12 mt-4">
                  <button className="text-5xl leading-3" id="prev">
                    ‹
                  </button>
                  <button className="text-5xl leading-5 " id="next">
                    ›
                  </button>
                </div>
              </div>
            </div>
          </swiper-slide>
        </swiper>
      </div>
    </div>
    <div className="flex flex-col lg:flex-row ">
      <div className="lg:w-4/12 flex flex-col" id="tokenomics">
        <div className="mt-36 mx-auto">
          <img src="../components/images/plane.png" className="banner-img" alt="" srcset="" />
        </div>
        <div>
          <h3 className="text-center text-4xl font-bold">
            Tokenomics <span className="text-[#7CCCEC]">V2</span>
          </h3>
          <div className="flex flex-col w-5/12 mx-auto text-2xl">
            <div className="flex flex-row justify-between">
              <p>Tax</p>
              <p>5%</p>
            </div>
            <div className="flex flex-row justify-between">
              <p>Operation</p>
              <p>1%</p>
            </div>
            <div className="flex flex-row justify-between">
              <p>Rewards</p>
              <p>4%</p>
            </div>
          </div>
        </div>
      </div>
      <div className="w-[2.5rem]"></div>
      <div className=" xl:w-4/12 lg:w-6/12 mt-20 lg:px-0 px-12 lg:mb-0 mb-20" id="roadmap">
        <h3 className="font-bold text-5xl">Roadmap</h3>
        <div className="flex flex-col border-l-[0.2rem] pl-4 border-[#D2D2D2] space-y-6 mt-6 sm:ml-12 ml-4">
          <div className="flex flex-row justify-between w-12/12">
            <div className="flex flex-col text-2xl">
              <p>MIGRATION TO METALABZ</p>
              <p className="text-[#C4C4C4]">
                Rebranding all socials and launching <br /> smart contract.
              </p>
            </div>
            <div className="text-[#7CCCEC] text-3xl">Stage 1</div>
          </div>
          <div className="flex flex-row justify-between w-12/12">
            <div className="flex flex-col text-2xl">
              <p>LAUNCH OF NEW PRE EXISTING DAPPS</p>
              <p className="text-[#C4C4C4]">
                Staking for NFTs token reward distrubiton <br /> pool rewards
                tracker.
              </p>
            </div>
            <div className="text-[#7CCCEC] text-3xl">Stage 2</div>
          </div>
          <div className="flex flex-row justify-between w-12/12">
            <div className="flex flex-col text-2xl">
              <p>LAUNCH 1ST NFT LABZ PRODUCT LINE</p>
              <p className="text-[#C4C4C4]">
                Unique implementation embedded within NFT <br /> structure.
              </p>
            </div>
            <div className="text-[#7CCCEC] text-3xl">Stage 3</div>
          </div>
          <div className="flex flex-row justify-between w-12/12">
            <div className="flex flex-col text-2xl">
              <p>ROLL OUT LIQUIDTY PROTOCOL-LIQUIDLABZ</p>
              <p className="text-[#C4C4C4]">
                Farms liquidty lending program liquidty <br /> assurance
                program.
              </p>
            </div>
            <div className="text-[#7CCCEC] text-3xl">Stage 4</div>
          </div>
          <div className="flex flex-row justify-between w-12/12">
            <div className="flex flex-col text-2xl">
              <p>AUTOMATED SMART CHECKER</p>
              <p className="text-[#C4C4C4]">
                First tool from DarkLabs more info to come
              </p>
            </div>
            <div className="text-[#7CCCEC] text-3xl">Stage 5</div>
          </div>
          <div className="flex flex-row justify-between w-12/12">
            <div className="flex flex-col text-2xl">
              <p>PUBLIC BETA METALABZ.GG LOBY</p>
              <p className="text-[#C4C4C4]">
                In addition to other game releases.
              </p>
            </div>
            <div className="text-[#7CCCEC] text-3xl">Stage 6</div>
          </div>
        </div>
      </div>
    </div>
    <div className="bg-[#A3A4EF] w-full p-8 my-12" id="subsidiaries">
      <h2 className="text-center sm:text-5xl text-3xl  text-white font-bold">
        Subsidiaries
      </h2>
      <div className="">
        <div className="">
          <swiper :modules="modules" :spaceBetween="50" :slidesPerView="1" :loop="true" @slideChange="handleSlideChange"
            @swiper="handleSwiper" :navigation="{ nextEl: '#next', prevEl: '#prev' }">
            <swiper-slide>
              <div className="flex flex-col">
                <div className="">
                  <div>
                    <img className="w-64 my-4 mx-auto" src="../components/images/nftlabz.png" alt="" />
                    <div
                      className="text-center text-black my-4 text-xl font-bold bg-[#7CCCEC] rounded-2xl sm:w-3/12 mx-auto  p-4">
                      <a className="text-white" href="http://nftlabz.app/">Go to nftlabz</a>
                    </div>
                  </div>
                  <div className="flex flex-row justify-between sm:w-1/12 mx-auto  my-8 text-white">
                    <button className="text-5xl leading-3" id="prev">
                      ‹
                    </button>
                    <button className="text-5xl leading-5 " id="next">
                      ›
                    </button>
                  </div>
                </div>
              </div>
            </swiper-slide>
            <swiper-slide>
              <div className="flex flex-col">
                <div className="">
                  <div>
                    <img className="w-64 mx-auto" src="../components/images/darklabz.png" alt="" />
                    <div
                      className="text-center text-black my-4 text-xl font-bold bg-[#7CCCEC] rounded-2xl w-3/12 mx-auto  p-4">
                      <a className="text-white" href="https://darklabz.com/">Go to darklabz</a>
                    </div>
                  </div>
                  <div className="flex flex-row justify-between w-1/12 mx-auto  my-8  text-white">
                    <button className="text-5xl leading-3" id="prev">
                      ‹
                    </button>
                    <button className="text-5xl leading-5 " id="next">
                      ›
                    </button>
                  </div>

                </div>
              </div>
            </swiper-slide> <swiper-slide>
              <div className="flex flex-col">
                <div className="">
                  <div>
                    <img className="w-64 mx-auto" src="../components/images/liquidlabz.png" alt="" />
                    <div
                      className="text-center text-black my-4 text-xl font-bold bg-[#7CCCEC] rounded-2xl w-3/12 mx-auto  p-4">
                      <a className="text-white" href="https://liquidlabz.com/">Go to liquidlabz</a>
                    </div>
                  </div>
                  <div className="flex flex-row justify-between w-1/12 mx-auto  my-8 text-white">
                    <button className="text-5xl leading-3" id="prev">
                      ‹
                    </button>
                    <button className="text-5xl leading-5 " id="next">
                      ›
                    </button>
                  </div>
                </div>
              </div>
            </swiper-slide>
            <swiper-slide>
              <div className="flex flex-col">
                <div className="">
                  <div>
                    <img className="w-64 mx-auto mt-10" src="../components/images/merchlabz.png" alt="" />
                    <div
                      className="text-center text-black my-4 text-xl font-bold bg-[#7CCCEC] rounded-2xl w-3/12 mx-auto  p-4">
                      <a className="text-white" href="http://merchlabz.com/">Go to merchlabz</a>
                    </div>
                  </div>
                  <div className="flex flex-row justify-between w-1/12 mx-auto  my-8 text-white">
                    <button className="text-5xl leading-3" id="prev">
                      ‹
                    </button>
                    <button className="text-5xl leading-5 " id="next">
                      ›
                    </button>
                  </div>
                </div>
              </div>
            </swiper-slide>

          </swiper>
        </div>
      </div>
    </div>
    <div className="flex flex-col lg:flex-row " id="partners">
      <div className="lg:w-4/12 flex flex-col">
        <div>
          <h3 className="text-center text-4xl font-bold">
            Meet our <span className="text-[#7CCCEC]">partners</span>
          </h3>
          <div className="flex flex-col w-7/12 mx-auto text-2xl">
            <div className="flex flex-row items-center">
              <img className="p-3" src="../components/images/pancakeswap-cake-logo.png" alt="" srcset="" />
              <p>Pancakeswap - listed</p>
            </div>
            <div className="flex flex-row items-center">
              <img className="p-3" src="../components/images/poocoin-poocoin-logo.png" alt="" srcset="" />
              <p>Poocoin - listed</p>
            </div>
            <div className="flex flex-row items-center">
              <img className="p-3" src="../components/images/gekko.png" alt="" srcset="" />
              <p>Coingekko - listed</p>
            </div>
            <div className="flex flex-row items-center">
              <img src="../components/images/0x0.png" alt="" srcset="" />
              <p>Coinmarketcap - listed</p>
            </div>
            <div className="flex flex-row items-center">
              <img src="../components/images/5866.png" alt="" srcset="" />
              <p>Dextools - listed</p>
            </div>
            <div className="flex flex-row items-center">
              <img className="p-3" src="../components/images/igW5IVrD_400x400.png" alt="" srcset="" />
              <p>Brewlabs - listed</p>
            </div>
          </div>
        </div>
      </div>
      <div className="w-[2.5rem]"></div>
      <div className="lg:w-5/12 lg:px-0 px-12">
        <h3 className="font-bold text-5xl mt-6" id="team">Meet the team</h3>

        <swiper :modules="modules" :spaceBetween="50" :slidesPerView="1" :loop="true" @slideChange="handleSlideChange"
          @swiper="handleSwiper" :navigation="{ nextEl: '#next', prevEl: '#prev' }">
          <swiper-slide>
            <div
              className="flex sm:flex-row flex-col justify-between lg:w-8/12 w-10/12 space-x-6 lg:space-x-0 space-y-6 mt-6 sm:ml-12">
              <div>
                <img className="" src="../components/images/final-home--1st.png" alt="" />
                <div className="flex flex-row  items-center">
                  <div>
                    <p className="px-4 pt-4 text-2xl">Chris Gin</p>
                    <p className="text-[#7CCCEC] px-4 text-4xl">Founder</p>
                  </div>
                  <div className="flex flex-row justify-between w-3/12">
                    <button className="text-5xl leading-3" id="prev">
                      ‹
                    </button>
                    <button className="text-5xl leading-5 " id="next">
                      ›
                    </button>
                  </div>
                </div>
              </div>
              <div className="xl:w-6/12  text-[#B5B5B5] sm:pt-10">
                <p className="lg:ml-4">
                  As founder it's my responsibility to guide the team in the
                  project to fulfill the vision we have laid out. I coordinate
                  all development and ensure ecosystem viability.
                </p>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div
              className="flex sm:flex-row flex-col justify-between lg:w-8/12 w-10/12 space-x-6 lg:space-x-0 space-y-6 mt-6 sm:ml-12">
              <div>
                <img src="../components/images/final-home--2nd.png" alt="" />
                <div className="flex flex-row  items-center">
                  <div>
                    <p className="px-4 pt-4 text-2xl">Nick</p>
                    <p className="text-[#7CCCEC] px-4 text-4xl">Co-Founder</p>
                  </div>
                  <div className="flex flex-row justify-between w-3/12">
                    <button className="text-5xl leading-3" id="prev">
                      ‹
                    </button>
                    <button className="text-5xl leading-5 " id="next">
                      ›
                    </button>
                  </div>
                </div>
              </div>
              <div className="xl:w-6/12  text-[#B5B5B5] sm:pt-10">
                <p className="lg:ml-4">
                  Nick is a vital member of the MBC team handling community engagement and all marketing oversight. He is
                  also a business liaison, and helps manage team partnerships.

                </p>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div
              className="flex sm:flex-row flex-col justify-between lg:w-8/12 w-10/12 space-x-6 lg:space-x-0 space-y-6 mt-6 sm:ml-12">
              <div>
                <img src="../components/images/final-home--3rd.png" alt="" />
                <div className="flex flex-row  items-center">
                  <div>
                    <p className="px-4 pt-4 text-2xl">Zubeysweet</p>
                    <p className="text-[#7CCCEC] px-4 text-4xl">Project Manager</p>
                  </div>
                  <div className="flex flex-row justify-between w-3/12">
                    <button className="text-5xl leading-3" id="prev">
                      ‹
                    </button>
                    <button className="text-5xl leading-5 " id="next">
                      ›
                    </button>
                  </div>
                </div>
              </div>
              <div className="xl:w-6/12  text-[#B5B5B5] sm:pt-10">
                <p className="lg:ml-4">
                  The person who will ensure that our project reaches the best places and who will manage our project.
                </p>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div
              className="flex sm:flex-row flex-col justify-between lg:w-8/12 w-10/12 space-x-6 lg:space-x-0 space-y-6 mt-6 sm:ml-12">
              <div>
                <img src="../components/images/final-home--4th.png" alt="" />
                <div className="flex flex-row  items-center">
                  <div>
                    <p className="px-4 pt-4 text-2xl">Steven Argyle Williamson</p>
                    <p className="text-[#7CCCEC] px-4 text-4xl">Lead VR dev</p>
                  </div>
                  <div className="flex flex-row justify-between w-3/12">
                    <button className="text-5xl leading-3" id="prev">
                      ‹
                    </button>
                    <button className="text-5xl leading-5 " id="next">
                      ›
                    </button>
                  </div>
                </div>
              </div>
              <div className="xl:w-6/12  text-[#B5B5B5] sm:pt-10">
                <p className="lg:ml-4">
                  Wargyle has worked in application development for AR and VR over numerous years and will be a integral
                  part of future development.

                </p>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div
              className="flex sm:flex-row flex-col justify-between lg:w-8/12 w-10/12 space-x-6 lg:space-x-0 space-y-6 mt-6 sm:ml-12">
              <div>
                <img src="../components/images/Luca.png" alt="" />
                <div className="flex flex-row  items-center">
                  <div>
                    <p className="px-4 pt-4 text-2xl">Luca</p>
                    <p className="text-[#7CCCEC] px-4 text-4xl"></p>
                  </div>
                  <div className="flex flex-row justify-between w-3/12">
                    <button className="text-5xl leading-3" id="prev">
                      ‹
                    </button>
                    <button className="text-5xl leading-5 " id="next">
                      ›
                    </button>
                  </div>
                </div>
              </div>
              <div className="xl:w-6/12  text-[#B5B5B5] sm:pt-10">
                <p className="lg:ml-4">

                </p>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div
              className="flex sm:flex-row flex-col justify-between lg:w-8/12 w-10/12 space-x-6 lg:space-x-0 space-y-6 mt-6 sm:ml-12">
              <div>
                <img src="../components/images/Kevin_Remer.png" alt="" />
                <div className="flex flex-row  items-center">
                  <div>
                    <p className="px-4 pt-4 text-2xl">Kevin Remer</p>
                    <p className="text-[#7CCCEC] px-4 text-4xl"></p>
                  </div>
                  <div className="flex flex-row justify-between w-3/12">
                    <button className="text-5xl leading-3" id="prev">
                      ‹
                    </button>
                    <button className="text-5xl leading-5 " id="next">
                      ›
                    </button>
                  </div>
                </div>
              </div>
              <div className="xl:w-6/12  text-[#B5B5B5] sm:pt-10">
                <p className="lg:ml-4">

                </p>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div
              className="flex sm:flex-row flex-col justify-between lg:w-8/12 w-10/12 space-x-6 lg:space-x-0 space-y-6 mt-6 sm:ml-12">
              <div>
                <img src="../components/images/Josh.png" alt="" />
                <div className="flex flex-row  items-center">
                  <div>
                    <p className="px-4 pt-4 text-2xl">Josh</p>
                    <p className="text-[#7CCCEC] px-4 text-4xl"></p>
                  </div>
                  <div className="flex flex-row justify-between w-3/12">
                    <button className="text-5xl leading-3" id="prev">
                      ‹
                    </button>
                    <button className="text-5xl leading-5 " id="next">
                      ›
                    </button>
                  </div>
                </div>
              </div>
              <div className="xl:w-6/12  text-[#B5B5B5] sm:pt-10">
                <p className="lg:ml-4">

                </p>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div
              className="flex sm:flex-row flex-col justify-between lg:w-8/12 w-10/12 space-x-6 lg:space-x-0 space-y-6 mt-6 sm:ml-12">
              <div>
                <img src="../components/images/marky.png" alt="" />
                <div className="flex flex-row  items-center">
                  <div>
                    <p className="px-4 pt-4 text-2xl">Marky</p>
                    <p className="text-[#7CCCEC] px-4 text-4xl"></p>
                  </div>
                  <div className="flex flex-row justify-between w-3/12">
                    <button className="text-5xl leading-3" id="prev">
                      ‹
                    </button>
                    <button className="text-5xl leading-5 " id="next">
                      ›
                    </button>
                  </div>
                </div>
              </div>
              <div className="xl:w-6/12  text-[#B5B5B5] sm:pt-10">
                <p className="lg:ml-4">

                </p>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div
              className="flex sm:flex-row flex-col justify-between lg:w-8/12 w-10/12 space-x-6 lg:space-x-0 space-y-6 mt-6 sm:ml-12">
              <div>
                <img src="../components/images/Ares.png" alt="" />
                <div className="flex flex-row  items-center">
                  <div>
                    <p className="px-4 pt-4 text-2xl">Ares</p>
                    <p className="text-[#7CCCEC] px-4 text-4xl"></p>
                  </div>
                  <div className="flex flex-row justify-between w-3/12">
                    <button className="text-5xl leading-3" id="prev">
                      ‹
                    </button>
                    <button className="text-5xl leading-5 " id="next">
                      ›
                    </button>
                  </div>
                </div>
              </div>
              <div className="xl:w-6/12  text-[#B5B5B5] sm:pt-10">
                <p className="lg:ml-4">

                </p>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div
              className="flex sm:flex-row flex-col justify-between lg:w-8/12 w-10/12 space-x-6 lg:space-x-0 space-y-6 mt-6 sm:ml-12">
              <div>
                <img src="../components/images/Dustin.png" alt="" />
                <div className="flex flex-row  items-center">
                  <div>
                    <p className="px-4 pt-4 text-2xl">Dustin</p>
                    <p className="text-[#7CCCEC] px-4 text-4xl"></p>
                  </div>
                  <div className="flex flex-row justify-between w-3/12">
                    <button className="text-5xl leading-3" id="prev">
                      ‹
                    </button>
                    <button className="text-5xl leading-5 " id="next">
                      ›
                    </button>
                  </div>
                </div>
              </div>
              <div className="xl:w-6/12  text-[#B5B5B5] sm:pt-10">
                <p className="lg:ml-4">

                </p>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div
              className="flex sm:flex-row flex-col justify-between lg:w-8/12 w-10/12 space-x-6 lg:space-x-0 space-y-6 mt-6 sm:ml-12">
              <div>
                <img className="w-20 h-20" src="../components/images/sistrictyfshift_final.png" alt="" />
                <div className="flex flex-row  items-center">
                  <div>
                    <p className="px-4 pt-4 text-2xl">Calvin Hofman aka Strxct</p>
                    <p className="text-[#7CCCEC] px-4 text-4xl">DEV OPS</p>
                  </div>
                  <div className="flex flex-row justify-between w-3/12">
                    <button className="text-5xl leading-3" id="prev">
                      ‹
                    </button>
                    <button className="text-5xl leading-5 " id="next">
                      ›
                    </button>
                  </div>
                </div>
              </div>
              <div className="xl:w-6/12  text-[#B5B5B5] sm:pt-10">
                <p className="lg:ml-4">
                  as the dev ops I make sure the servers stay up to date and that all the sites are being made and
                  deployed
                </p>
              </div>
            </div>
          </swiper-slide>
        </swiper>
      </div>
    </div>
    <div className="flex lg:flex-row flex-col ">
      <div className="lg:w-4/12 flex flex-col lg:px-0 sm:px-12" id="contact">
        <div>
          <h3 className="text-center text-4xl font-bold mt-8">
            Contact <span className="text-[#7CCCEC]">us</span>
          </h3>
          <div className="flex flex-col xl:w-5/12 lg:w-9/12 w-7/12 mx-auto text-2xl">
            <div className=" invisible" id="notify"></div>
            <form ref="form" @submit.prevent="sendEmail">
              <div className="flex flex-col">
                <label htmlFor="">Your name</label>
                <input className="border-2 border-[#E0E0E0]" type="text" name="name" id="name" />
              </div>
              <div className="flex flex-col">
                <label htmlFor="">Telegram username</label>
                <input className="border-2 border-[#E0E0E0]" type="text" name="telegram" id="telegram" />
              </div>
              <div className="flex flex-col">
                <label htmlFor="">Email</label>
                <input className="border-2 border-[#E0E0E0]" type="text" name="email" id="email" />
              </div>
              <div className="flex flex-col">
                <label htmlFor="">Subject</label>
                <input className="border-2 border-[#E0E0E0]" type="text" name="subject" id="subject" />
              </div>
              <div className="flex flex-col">
                <label htmlFor="">Message</label>
                <textarea className="border-2 border-[#E0E0E0]" name="message" id="message" cols="20" rows="4"></textarea>
              </div>
              <button type="submit" value="Send" className="text-[#7CCCEC]">
                Send message <span className="text-4xl ">›</span>
              </button>
            </form>
          </div>
        </div>
      </div>
      <div className="w-[2.5rem]"></div>
      <div className=" xl:w-5/12 lg:w-8/12 lg:px-0 px-12" id="buy">
        <h3 className="font-bold text-5xl mt-6">Buy now</h3>
        <div className="flex flex-row justify-between lg:w-8/12 space-y-6 mt-6">
          <iframe className="sm:w-11/12 w-full h-[600px] sm:h-[725px]"
            src="https://v3app.everrise.com/everswap/?embedded=1&mode=light#chainId=56&token=0xf14d3692b0055db9ca4c04065165d59b87e763f1&stripMode=true"
            frameborder="0"></iframe>
        </div>
      </div>
    </div>

    <div className="bg-[#A3A4EF] p-8 mt-40">
      <div className="flex sm:flex-row flex-col justify-between  items-center">
        <div className="flex flex-col p-12 space-y-2">
          <div>
            <p className="text-4xl text-white ">
              Documents
            </p>
          </div>
          <div>
            <a href="../components/images/WhitePaper_1.pdf" target="_blank" className="text-2xl text-white ">
              Whitepaper
            </a>
          </div>

          <div>
            <a href="../components/images/audit_1.pdf" target="_blank" className="text-2xl text-white ">
              Audit - interfi
            </a>
          </div>



        </div>
        <div className="flex flex-row justify-between w-full lg:w-3/12 sm:w-7/12 sm:p-12">
          <div>
            <a href="https://twitter.com/MetaBusdCoin">
              <img src="../components/images/Icon awesome-twitter-white.png" alt="" />
            </a>
          </div>
          <div>
            <a href="https://www.reddit.com/r/MetaBUSDCoin/">
              <img src="../components/images/Icon awesome-reddit-alien-white.png" alt="" />
            </a>
          </div>
          <div>
            <a href="https://t.me/+U8iy18bIQdk0M2Zh">
              <img src="../components/images/Icon awesome-telegram-plane-white.png" alt="" />
            </a>
          </div>
          <div>
            <a href="https://discord.com/invite/r2YU2nPnHj">
              <img src="../components/images/Icon simple-discord-white.png" alt="" />
            </a>
          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
import emailjs from '@emailjs/browser';
import { Navigation, Pagination } from 'swiper/modules';
import { RouterLink } from 'vue-router'


import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';
import 'swiper/css/navigation';
import 'swiper/css/pagination';
import 'swiper/css/scrollbar';
// import { Swiper, SwiperSlide } from 'swiper/vue';
// import 'swiper/css';


export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    const onSwiper = (swiper) => {
      console.log(swiper);
    };
    const onSlideChange = () => {
      console.log('slide change');
    };
    return {
      onSwiper,
      onSlideChange,
      modules: [Navigation, Pagination],
    };
  },
  data() {
    return {
      isOpen: true,
      isActive: true,
      showSuccess: false,
      successMessage: "",
    };
  },
  methods: {
    handleSlideChange() {
      console.log('slide change');
    },
    closeModal() {
      this.isOpen = false;
    },
    handleClick(forceOpen = undefined) {
      if (forceOpen !== undefined) {
        this.isActive = forceOpen;
      } else {
        this.isActive = !this.isActive;
      }
    },
    navbarLinking() {
      // Handle navbar linking
    },

    sendEmail() {
      let counter = 0;

      if (this.$refs.form.name.value === "") {
        this.showSuccess = true;
        this.successMessage = "Fill in the name.";
      } else {
        counter++;
      }

      if (this.$refs.form.telegram.value === "") {
        this.showSuccess = true;
        this.successMessage = "Fill in the telegram.";
      } else {
        counter++;
      }

      if (this.$refs.form.email.value === "") {
        this.showSuccess = true;
        this.successMessage = "Fill in the email.";
      } else {
        counter++;
      }

      if (this.$refs.form.subject.value === "") {
        this.showSuccess = true;
        this.successMessage = "Fill in the subject.";
      } else {
        counter++;
      }

      if (this.$refs.form.message.value === "") {
        this.showSuccess = true;
        this.successMessage = "Fill in the message.";
      } else {
        counter++;
      }

      if (counter === 5) {
        emailjs
          .sendForm(
            "service_nm0tssk",
            "template_s8ck84z",
            this.$refs.form,
            "user_qBzdCt1PnXVUhV66FcLnK"
          )
          .then(
            (result) => {
              console.log(result.text);
              this.$refs.form.subject.value = "";
              this.$refs.form.message.value = "";
              this.$refs.form.email.value = "";
              this.$refs.form.telegram.value = "";
              this.$refs.form.name.value = "";
              this.showSuccess = true;
              this.successMessage = "Email sent!";
            },
            (error) => {
              console.log(error.text);
            }
          );
      }
    }
  },
};
</script>
