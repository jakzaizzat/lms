<template>
    <VueSignaturePad
        id="signature"
        width="500px"
        height="500px"
        ref="signaturePad"
    />
</template>


<style>

#signature {
  border: double 3px transparent;
  border-radius: 5px;
  background-image: linear-gradient(white, white),
    radial-gradient(circle at top left, #4bc5e8, #9f6274);
  background-origin: border-box;
  background-clip: content-box, border-box;
}

</style>
