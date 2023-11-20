<script>
  // let files;

  // $: if (files) {
  //   // Note that `files` is of type `FileList`, not an Array:
  //   // https://developer.mozilla.org/en-US/docs/Web/API/FileList

  //   console.log(files);

  //   for (const file of files) {
  //     const body = new FormData();
  //     body.append("file", file);

  //     fetch("http://localhost:8080/upload?path=/", {
  //       body,
  //       headers: {
  //         "Content-Type": "multipart/form-data",
  //       },
  //     });
  //   }
  // }
  // let files;
  // let dataFile = null;
  // function upload() {
  //   const formData = new FormData();
  //   formData.append("damName", value);
  //   formData.append("dataFile", files[0]);
  //   const upload = fetch("http://localhost:8080/upload?path=/", {
  //     method: "POST",
  //     body: formData,
  //   })
  //     .then((response) => response.json())
  //     .then((result) => {
  //       console.log("Success:", result);
  //     })
  //     .catch((error) => {
  //       console.error("Error:", error);
  //     });
  // }


  // const authorizedExtensions = ['.jpg', '.jpeg', '.png', '.webp'];
</script>


<form action="http://localhost:8080/upload?path=/" method="post" enctype="multipart/form-data">
  <input type="file" name="avatar" placeholder="avatar" />
  <button type="submit">upload</button>
</form>

<form action="http://localhost:8080/upload?path=/" method="post" enctype="multipart/form-data">
  <input type="hidden" name="mkdir" value="test2"/>
  <button type="submit">create</button>
</form>