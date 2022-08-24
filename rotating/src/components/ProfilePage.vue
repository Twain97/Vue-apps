<template>
  <div class="container"></div>
</template>

<script>
export default {
  name: "ProfilePage",
};
</script>

<style  scoped>
* {
  margin: 0;
  padding: 0;
}
.container {
  position: relative;
  /* border: 4px solid rgb(121, 116, 116); */
  margin: 0 auto;
  width: 32%;
  height: 80vh;
  overflow: hidden;
  border-radius: 20px;
}
.container::before {
  content: "";
  position: absolute;
  top: -35%;
  left: 25%;
  width: 50%;
  height: 140vh;
  transform: rotate(15deg);
  animation: round 4500ms linear infinite;
  background: linear-gradient(
    rgb(18, 195, 207) 25%,
    rgb(11, 2, 17),
    rgb(18, 195, 207) 25%
  );
}
.container::after {
  content: "";
  position: absolute;
  /* display: flex;
  align-content: center;
  justify-content: center; */
  width: 98%;
  height: 79vh;
  left: 50%;
  top: 50%;
  background-color: rgb(14, 16, 19);
  border-radius: 20px;
  transform: translate(-50%, -50%);
  /* box-shadow: 4px 4px 12px gray, -4px -4px 12px gray; */
}

@keyframes round {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}

/************** Mobile Version **************************/
@media (max-width: 480px) {
  .container {
    position: relative;
    /* border: 4px solid rgb(121, 116, 116); */
    margin: 0 auto;
    width: 70%;
    height: 80vh;
    overflow: hidden;
    border-radius: 20px;
    z-index: 1;
  }
  .container::before {
    content: "";
    position: absolute;
    top: -35%;
    left: 25%;
    width: 50%;
    height: 140vh;
    transform: rotate(15deg);
    animation: round 4500ms linear infinite;
    background: linear-gradient(
      rgb(18, 195, 207) 25%,
      rgb(11, 2, 17),
      rgb(18, 195, 207) 25%
    );
  }
  .container::after {
    content: "";
    position: absolute;
    display: flex;
    align-content: center;
    justify-content: center;
    width: 98%;
    height: 78.9vh;
    left: 50%;
    top: 50%;
    background-color: rgb(14, 16, 19);
    border-radius: 20px;
    transform: translate(-50%, -50%);
  }

  @keyframes round {
    from {
      transform: rotate(0deg);
    }
    to {
      transform: rotate(360deg);
    }
  }
}
</style>