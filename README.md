<div>
  <h2>QA Engineer Portfolio: Vehicle Registered State Validation</h2>
  <p><strong>Company:</strong> General Insurance INC.</p>
  <p>
    As a QA Engineer at General Insurance INC., I have conducted thorough test cases to verify the validation of vehicle registered states. This project focused on ensuring that the vehicle creation endpoint correctly handles various scenarios related to state validation, maintaining data integrity, and adhering to the required specifications.
  </p>

  <h3>Test Case Outline:</h3>
  <ol>
    <li>Verify that the user is able to successfully create a new vehicle with a valid registered state. Status code 201 received.</li>
    <li>Send a request with a registered state as 'CA', API should process it successfully.</li>
    <li>Send a request with a registered state as California, API should process it successfully.</li>
    <li>Send a request with an invalid registered state name such as 'Berlin', API must render an error with status code 400.</li>
  </ol>

  <h3>Test Case Results:</h3>
  
  <!-- Test Case 1 -->
  <table border="1">
    <thead>
      <tr>
        <th colspan="4">Test Case ID: TC01</th>
      </tr>
      <tr>
        <th>API Body</th>
        <th>Expected Result</th>
        <th>Actual Result</th>
        <th>Status Code</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
          {
            "year": "2022",
            "Make": "Toyota",
            "Trim": "LTZ",
            "Mileage": 23236,
            "numberplate": "KUO138",
            "registeredstate": "New York",
            "createdDate": "2022-06-18T00:00:00.000Z",
            "vin": 69527781600,
            "Model": "MRK",
            "Color": "White"
          }
        </td>
        <td>Verify that the user can successfully create a new vehicle with a valid registered state. Status code 201 received.</td>
        <td>I verified that the user can successfully create a new vehicle with a valid registered state. Status code 201 received.</td>
        <td>Status code 201 received.</td>
      </tr>
      <tr>
        <td colspan="4"><img src="https://github.com/user-attachments/assets/6083ab94-b283-4abd-837f-dd07e34cbb0b" width="1000" height="500" alt="Test Case 1"></td>
      </tr>
    </tbody>
  </table>
  <br><br><br>
  
  <!-- Test Case 2 -->
  <table border="1">
    <thead>
      <tr>
        <th colspan="4">Test Case ID: TC02</th>
      </tr>
      <tr>
        <th>API Body</th>
        <th>Expected Result</th>
        <th>Actual Result</th>
        <th>Status Code</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
          {
            "year": "2022",
            "Make": "Toyota",
            "Trim": "LTZ",
            "Mileage": 23236,
            "numberplate": "KUO138",
            "registeredstate": "CA",
            "createdDate": "2022-06-18T00:00:00.000Z",
            "vin": 69527781611,
            "Model": "MRK",
            "Color": "White"
          }
        </td>
        <td>Send a request with a registered state as 'CA' API should process it successfully. Status code 201 received.</td>
        <td>I sent a request with a registered state as 'CA' and the API processed it successfully. Status code 201 received.</td>
        <td>Status code 201 received.</td>
      </tr>
      <tr>
        <td colspan="4"><img src="https://github.com/user-attachments/assets/cee94db1-711d-4bb3-be6c-0ad3c28e855d" width="1000" height="500" alt="Test Case 2"></td>
      </tr>
    </tbody>
  </table>
  <br><br><br>
  
  <!-- Test Case 3 -->
  <table border="1">
    <thead>
      <tr>
        <th colspan="4">Test Case ID: TC03</th>
      </tr>
      <tr>
        <th>API Body</th>
        <th>Expected Result</th>
        <th>Actual Result</th>
        <th>Status Code</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
          {
            "year": "2022",
            "Make": "Toyota",
            "Trim": "LTZ",
            "Mileage": 23236,
            "numberplate": "KUO138",
            "registeredstate": "California",
            "createdDate": "2022-06-18T00:00:00.000Z",
            "vin": 69527781622,
            "Model": "MRK",
            "Color": "White"
          }
        </td>
        <td>Send a request with a registered state as California API should process it successfully. Status code 201 received.</td>
        <td>I sent a request with a registered state California API processed it successfully. Status code 201 received.</td>
        <td>Status code 201 received.</td>
      </tr>
      <tr>
        <td colspan="4"><img src="https://github.com/user-attachments/assets/fdad27fd-ba3c-4f52-a929-92a6238f6a82" width="1000" height="500" alt="Test Case 3"></td>
      </tr>
    </tbody>
  </table>
  <br><br><br>

  <!-- Test Case 4 -->
  <table border="1">
    <thead>
      <tr>
        <th colspan="4">Test Case ID: TC04</th>
      </tr>
      <tr>
        <th>API Body</th>
        <th>Expected Result</th>
        <th>Actual Result</th>
        <th>Status Code</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
          {
            "year": "2022",
            "Make": "Toyota",
            "Trim": "LTZ",
            "Mileage": 23236,
            "numberplate": "KUO138",
            "registeredstate": "Berlin",
            "createdDate": "2022-06-18T00:00:00.000Z",
            "vin": 695277816115,
            "Model": "MRK",
            "Color": "White"
          }
        </td>
        <td>Send a request with an invalid registered state name such as ‘Berlin’ API must render an error with status code 400.</td>
        <td>I sent a request with the invalid registered state name 'Berlin' and the API rendered an error with status code 400.</td>
        <td>Status code 400 received.</td>
      </tr>
      <tr>
        <td colspan="4"><img src="https://github.com/user-attachments/assets/785bd8f7-55e4-44c1-a81f-42cda8928823" width="1000" height="500" alt="Test Case 4"></td>
      </tr>
    </tbody>
  </table>
  <br><br><br>
</div>
