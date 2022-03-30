# WEBAPI
using System;
using System.Collections.Generic;
using System.Linq;
using System.Net;
using System.Net.Http;
using System.Web.Http;

namespace WebApiFirstProject.Controllers
{
    public class EmpController : ApiController
    {
        [HttpGet]

        [Route("Std/Student")]

        public List<string> GetEmp()
        {
           
            List<string> objlist = new List<string>()
            {

                "Abhishek",
                "Test",
                "Chetu",
                "Anjali"

            };

            return objlist;
        }

        [HttpPost]
        [Route("Abhi/Student")]
        public string PostEmp()
        {


            string str = "Abhi";

            return str;

        }

        [HttpPost]
        [Route("Abhi/Student")]
        public void PostEmpl()
        {

        }

    }
}
