<template>
  <div class="live-online">
    <strong>LIVE ONLINE COURSE</strong>

    <strong class="hide-sm">LIVE ONLINE COURSE</strong>
    <strong class="hide-sm">LIVE ONLINE COURSE</strong>
    <strong class="hide-md">LIVE ONLINE COURSE</strong>
  </div>
</template>

<style scoped>
.live-online {
  width: 100%;
  background-color: #FE5D34;
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  justify-content: space-evenly;
  align-items: center;
  padding: 10px;
  font-family: Nekst, sans-serif;
  margin:  auto 0;

}

.live-online strong {
  font-weight: 400;
  font-size: clamp(12px, 2vw, 20px);
  white-space: nowrap;
}

/* hide some items on smaller screens */
@media (max-width: 768px) {
  .hide-sm {
    display: none;
  }
}

@media (max-width: 480px) {
  .hide-md {
    display: none;
  }
}
</style>
