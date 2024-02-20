<script>
import MainHero from '@/components/MainHero.vue'
import MainSection from '@/components/MainSection.vue'
import TitleSection from '@/components/TitleSection.vue'
import CardOverlay from '@/components/CardOverlay.vue'
export default {
  name: 'HomeView',
  components: {
    MainHero,
    MainSection,
    TitleSection,
    CardOverlay
  }
}
</script>

<template>
  <main>
    <MainHero description="Click below to try it out for completely free!" buttonText="Learn More"
      buttonTarget="#more-info" />
    <div class="grid grid-cols-3 justify-between py-8 px-5 w-4/5 mx-auto">
      <div id="more-info" class="col-span-2">
        <MainSection title="Saves you time"
          description="Without a booking system, booking can be a major hassle. A booking system not only saves you time by not having to manage something as time consuming as booking, but also increases clarity. No more having to constantly go back in forth with multiple people regarding scheduling." />
        <MainSection title="Built in scheduling"
          description="Scheduling is easy to set up. All you have to do is specify the hours you are available for booking, and then your client selects them." />
        <MainSection title="Customizable"
          description="You can customize your booking system to fit your needs. You can set up your booking system to have different services, different time slots, and different staff members." />
        <MainSection title="Easy to use"
          description="The booking system is easy to use for both you and your clients. It is easy to set up, and easy to use. Your clients will have no problem booking with you." />
        <MainSection title="Mobile friendly"
          description="The booking system is mobile friendly. Your clients can book with you from anywhere, at any time." />
        <MainSection title="Secure"
          description="The booking system is secure. Your clients can book with you without having to worry about their information being compromised." />
        <MainSection title="Affordable"
          description="The booking system is affordable. You can have a booking system for your business without breaking the bank." />
        <div class="border border-primary pt-2 rounded-box">
          <h2 class="text-center text-5xl font-semibold underline">Coming Soon</h2>
          <div class="grid grid-flow-col">
            <TitleSection title="Frequent Updates"
              description="We are constantly updating our booking system to make sure it is the best it can be." />
            <TitleSection title="Google Calendar Integration"
              description="We are working on integrating Google Calendar into our booking system." />
          </div>
        </div>
      </div>
      <div class="col-span-1 flex flex-col bg-base-200 p-5 mx-auto rounded-box justify-around">
        <CardOverlay title="The Benefits of Online Booking Systems"
          description="Read this article about how important online booking systems are." buttonText="Read Article"
          buttonTarget="https://www.clock-software.com/blog/benefits-of-online-booking-systems" />
        <CardOverlay />
        <CardOverlay />
        <CardOverlay />
      </div>
    </div>
  </main>
</template>

<style>
html {
  scroll-behavior: smooth;
}
</style>