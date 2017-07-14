**Generate Image**
----
  Returns an custom dummy image.

* **URL**

  /generate

* **Method:**

  `GET`

*  **URL Params**

   **Optional:**

   `width=[integer]`

   **Optional:**

   `height=[integer]`

   **Optional:**

   `color=[string]`

   **Optional:**

   `caption=[string]`   


* **Data Params**

  None

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `{ imgUrl : "http://my.image.sample" }`

* **Error Response:**

  * **Code:** 404 NOT FOUND <br />
    **Content:** `{ error : "Could not generate the image" }`

* **Sample Call:**

  ```javascript
    $.ajax({
      url: "/generate",
      dataType: "json",
      type : "GET",
      success : function(r) {
        console.log(r);
      }
    });
  ```
