<!DOCTYPE html>
<!--[if lt IE 7]>      <html class="no-js lt-ie9 lt-ie8 lt-ie7"> <![endif]-->
<!--[if IE 7]>         <html class="no-js lt-ie9 lt-ie8"> <![endif]-->
<!--[if IE 8]>         <html class="no-js lt-ie9"> <![endif]-->
<!--[if gt IE 8]><!-->
<html class="no-js">
<!--<![endif]-->

<head>
    <meta charset="utf-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <title></title>
    <meta name="description" content="" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <link rel="stylesheet" href="app.styles.css" />
</head>

<body>
    <!--[if lt IE 7]>
      <p class="browsehappy">
        You are using an <strong>outdated</strong> browser. Please
        <a href="#">upgrade your browser</a> to improve your experience.
      </p>
    <![endif]-->

    <div class="container">
        <div class="form-container">
            <form class="application">
                <fieldset>
                    <legend>iteach Account Creation:</legend>
                    <div class="grid">
                        <div class="grid-item">
                            <label for="useremail">Email:</label><br/>
                            <input type="email" id="useremail" name="useremail"/>
                        </div>
                        <div class="grid-item">
                            <label for="confirmemail">Confirm Email:</label><br/>
                            <input type="email" id="confirmemail" name="confirmemail"/>
                        </div>
                        <div class="grid-item">
                            <label for="hearaboutus">How did you hear about us?:</label><br/>
                            <select id="hearaboutus" name="hearaboutus">
                                <option value="referral">Referral</option>
                                <option value="job/career fair">Job Fair/Career Fair</option>
                                <option value="kellyservices">Kelly Services</option>
                                <option value="schooldistrict">School District</option>
                                <option value="facebook">Facebook</option>
                                <option value="linkedin">LinkedIn</option>
                                <option value="twitter">Twitter</option>
                                <option value="bingsearch">Bing Search</option>
                                <option value="googlesearch">Google Search</option>
                            </select>
                        </div>
                        <div class="grid-item">
                            <label for="userpassword">Password:</label><br/>
                            <input type="password" id="userpassword" name="userpassword"/>
                        </div>
                        <div class="grid-item">
                            <label for="confirmpassword">Confirm Password:</label><br/>
                            <input type="password" id="confirmpassword" name="confirmpassword"/>
                        </div>

                    </div>
                </fieldset>
                <fieldset class="personal-info">
                    <legend>Personal Information:<br/>
                    <span class="subtitle">Please list Legal Name as seen on Photo ID.</span></legend>
                    <div class="grid">
                        <div class="grid-item">
                            <label for="fname">First Name:</label><br />
                            <input type="text" id="fname" name="fname" />
                        </div>
                        <div class="grid-item">
                            <label for="minit">Middle Initial:</label><br />
                            <input type="text" id="minit" name="minit" />
                        </div>
                        <div class="grid-item">
                            <label for="lname">Last Name:</label><br />
                            <input type="text" id="lname" name="lname" />
                        </div>

                        <div class="grid-item">
                            <label for="lname">Maiden Name:</label><br />
                            <input type="text" id="mname" name="mname" />
                        </div>


                        <div class="grid-item">
                            <label for="minit">Birthdate:</label><br />
                            <input type="date" id="minit" name="minit" />
                        </div>

                        <div class="grid-item">
                            <label for="minit">Social Security Number:</label><br />
                            <input type="tel" id="minit" name="minit" pattern="[0-9]{3}-[0-9]{2}-[0-9]{4}" />
                        </div>

                        <div class="grid-item">
                            <label for="gender">Gender:</label><br />
                            <select id="gender" name="gender">
                                <option value="male">Male</option>
                                <option value="female">Female</option>
                                <option value="nondisclosed">Rather not say</option>
                            </select>
                        </div>
                    </div>
                </fieldset>

                <fieldset>
                    <legend>Contact Information:</legend>
                    <div class="grid">

                        <div class="address grid-item">
                            <div class="address-grid-item">
                                <label for="homeaddress">Address:</label><br />
                                <input type="text" id="homeaddress" name="homeaddress" />
                            </div>

                            <div class="address-grid-item">
                                <label for="city">City:</label><br />
                                <input type="text" id="city" name="city" />
                            </div>

                            <div class="address-grid-item">
                                <label for="state">State:</label><br />
                                <select id="state" name="state"></select>
                            </div>

                            <div class="address-grid-item">
                                <label for="zip">Zipcode:</label><br />
                                <input type="text" id="zip" name="zip" />
                            </div>
                        </div>

                        <div class="grid-item">
                            <label for="phone" pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}">Phone Number:</label> <br />
                            <input type="tel" id="phone" name="phone" />
                        </div>
                        <div class="grid-item">
                            <label for="email" >Email Address:</label> <br />
                            <input type="email" id="email" name="email" />
                        </div>

                    </div>
                </fieldset>

                <fieldset>
                    <legend>Citizenship and Ethnicity Information:</legend>
                    <div class="grid">
                       

                        <div class="grid-item">
                            <label for="uscitizen">Are you a US Citizen?</label><br />
                            <select id="uscitizen" name="uscitizen" onchange="workVisa()">
                                <option value="yes">Yes</option>
                                <option value="no">no</option>
                            </select>
                        </div>
                        
                        <div class="grid-item" id="eligible">
                            <label for="uswork">Are you eligible to work in the United States?</label><br />
                            <select id="uswork" name="uswork">
                                <option value="yes">Yes</option>
                                <option value="no">no</option>
                            </select>
                        </div>
                        <div class="grid-item">
                            <label for="military">Are you a veteran or active military?</label><br />
                            <select id="military" name="military">
                                <option value="yes">Yes</option>
                                <option value="no">no</option>
                            </select>
                        </div>
                        <div class="grid-item">
                            <label for="ethnicity">Ethnicity:</label><br />
                            <Select type="" id="ethnicity" name="ethnicity">
                                <option value="">White/Causasian</option>
                                <option value="">American Indian or Alaska Native</option>
                                <option value="">Asian</option>
                                <option value="">Black or African American</option>
                                <option value="">Hispanic/Latino</option>
                                <option value="">Native Hawaiian or Pacific Islander</option>
                                <option value="">Other</option>
                            </Select>
                        </div>
                        <div class="grid-item">
                            <label for="hispanic">Are you Hispanic/Latino? Yes?</label>
                            <input type="checkbox" id="hispanic" name="hispanic" />
                        </div>
                    </div>
                </fieldset>
                <fieldset>
                    <legend>Certification Information:</legend>
                    <div class="grid">
                        <div class="grid-item">
                            <label for="certtype">Certification Type:</label>
                            <select id="certtype" name="certtype" onchange="interestArea()">
                                <option value="default">Please Choose</option>
                                <option value="teacher">Teacher</option>
                                <option value="principal">Principal</option>
                            </select>
                        </div>

                        <div class="grid-item">
                            <label for="certstate">Certification State:</label><br />
                            <select id="certstate" name="certstate" onchange="interestArea()">
                                <option value="default">Please Choose</option>
                                <option value="texas">Texas</option>
                                <option value="nevada">Nevada</option>
                                <option value="other-states">Other States</option>
                            </select>
                        </div>
                        <div class="grid-item" id="program-area">
                            <label for="programarea">Program Area of interest:</label><br />
                            <select id="programarea" name="programarea">
                                <option value="elementary">Elementary</option>
                                <option value="secondary">Secondary</option>
                                <option value="special">Special Education</option>
                            </select>
                            
                        </div>
                        <div class="grid-item" id="content-area">
                            <label for="contentarea">Content Area of interest:</label><br />
                            <select id="contentarea" name="conteantarea">
                                <option value="placeholder">Big List Here</option>
                                
                            </select>
                            
                        </div>
                       
                        
                        <div class="grid-item">
                            <label for="otherprog">Have you ever been enrolled in another teacher prep program? Yes?</label>
                            <input type="checkbox" id="otherprog" name="otherprog" />
                        </div>
                        <div class="grid-item">
                            <label for="districtoffer">Has a district already made you an offer to teach? Yes?</label>
                            <input type="checkbox" id="districtoffer" name="districtoffer" />
                        </div>
                    </div>
                </fieldset>
                <fieldset>
                    <legend>Education Information:</legend>
                    <div class="grid outer-education-block">
                        <div class="grid-item">
                            <label for="conferreddegree">Do you have a conferred degree?</label><br/>
                            <select id="conferreddegree" name="conferreddegree" onchange="askDate()">
                                <option value='yes'>Yes</option>
                                <option value='no'>No</option>
                            </select>
                        </div>
                        <div class="grid-item" id="grad-date-div">
                            <label for="graddate">Expected graduation date:</label><br />
                            <input type="date" id="graddate" name="graddate" />
                        </div>
                    
                            <div class="grid grid-item education-block">
                                <div class="grid-item">
                                    <label for="college">College/University Attended:</label><br/>
                                    <input type="" id="college" name="college"/>
                                </div>
                                <div class="grid-item">
                                    <label for="major">Major Earned:</label><br/>
                                    <input type="text" id="major" name="major"/>
                                </div>
                                <div class="grid-item">
                                    <label for="degree">Degree Awarded(BA,BS,MA,ect.):</label><br/>
                                    <input type="text" id="degree" name="degree"/>
                                </div>
                                <div class="grid-item">
                                    <label for="graddate">Last Date Attended/Date of Graduation:</label><br/>
                                    <input type="date" id="graddate" name="graddate"/>
                                </div>
                                <button class="grid-item">Add More Education</button>
                            </div>
                    </div>
                    
                </fieldset>
                <fieldset>
                    <legend>Employment Informaton:</legend>
                    <div class="grid work-block">
                        <div class="grid-item">
                            <label for="employer">Employer:</label><br>
                            <input type="text" id="employer" name="employer" />
                        </div>
                        <div class="grid-item">
                            <label for="position">Position:</label><br/>
                            <input type="text" id="position" name="position" />
                        </div>
                        <div class="grid-item">
                            <label for="fromdate">From:</label><br/>
                            <input type="date" id="fromdate" name="fromdate" />
                        </div>
                        <div class="grid-item">
                            <label for="todate">To:</label><br/>
                            <input type="date" id="todate" name="todate" />
                        </div>

                    </div>
                    <button class="grid-item">Add More Work History</button>
                </fieldset>
               
            </form>
        </div>
    </div>

    <script src="app.scripts.js" defer></script>
</body>

</html>