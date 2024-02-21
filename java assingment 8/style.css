
function simulateAsyncOperation(shouldSucceed) {
    return new Promise((resolve, reject) => {
      setTimeout(() => {
        if (shouldSucceed) {
          resolve("success");
        } else {
          reject(new Error("Error"));
        }
      }, 3000);
    });
  }
  
  simulateAsyncOperation(true)
    .then((success) => {
      console.log(success);
    })
    .catch((error) => {
      console.error(error.message);
    });

  simulateAsyncOperation(false)
    .then((success) => {
      console.log(success);
    })
    .catch((error) => {
      console.error(error.message);
    });


function fetchData() {
    return new Promise((resolve, reject) => {
      setTimeout(() => {
        const data = { message: "Data Fetched" };
        resolve(data);
      }, 4000);
    });
  }
  
  function processData(data) {
    return new Promise((resolve, reject) => {
      setTimeout(() => {
        const processedData = { message: "Data process Completed", originalData: data };
        resolve(processedData);
      }, 3500); 
    });
  }
  
  fetchData()
    .then((fetchedData) => {
      console.log("Data fetched:", fetchedData);
      return processData(fetchedData);
    })
    .then((processedData) => {
      console.log("Data processed:", processedData);
      console.log("Final result:", processedData);
    })
    .catch((error) => {
      console.error("Error:", error);
    });