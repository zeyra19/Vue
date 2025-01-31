onMounted(async() => {
        try {
          const response = await fetch("https://jsonplaceholder.typicode.com/todos/")
          const data: Todo[] = await response.json();
          todos.value = data;         
        } catch (error) {
          console.log("hata oluştu", error)
        }
      });

