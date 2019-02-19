using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using VotingSystem.data;
using VotingSystem.data.DAO;
using VotingSystem.data.IDAO;
using VotingSystem.Services.IService;

namespace VotingSystem.Services.Service
{
   public class VotingSystemService :
        VotingSystem.Services.IService.IVotingSystemService
       
    {
        private VotingSystemDAO _votingSystemDAO;

        public VotingSystemService()
        {
            _votingSystemDAO = new VotingSystemDAO();
        }


        public IList<Topic_Recording> GetTopicRecordings()
        {
            return _votingSystemDAO.GetTopicRecordings();
        }

        public Topic_Recording GetTopicDetails(int id)
        {
            return _votingSystemDAO.GetTopicDetails(id);
        }
        public IList<Topic_Recording> GetTopicRecording()
        {
            return _votingSystemDAO.GetTopicRecordings();
        }

        public void CreateTopic(Topic_Recording topic)
        {
            _votingSystemDAO.CreateTopic(topic);
        }

        public void EditTopic(Topic_Recording topic)
        {
            _votingSystemDAO.EditTopic(topic);
        }

        public void DeleteTopic(Topic_Recording topic)
        {
            _votingSystemDAO.DeleteTopic(topic);
        }







        public IList<User_Recording> GetUserRecordings()
        {
            return _votingSystemDAO.GetUserRecordings();
        }
        public User_Recording GetUserDetails(int id)
        {
            return _votingSystemDAO.GetUserDetails(id);
        }

        public IList<User_Recording> GetUserRecording()
        {
            return _votingSystemDAO.GetUserRecordings();
        }

        public void UserRegister(User_Recording user)
        {
            _votingSystemDAO.UserRegister(user);
        }

        public void EditUser(User_Recording user)
        {
            _votingSystemDAO.EditUser(user);
        }


        public IList<User_Recording> GetAdministratorRecordings()
        {
            return _votingSystemDAO.GetAdministratorRecordings();
        }

        public User_Recording GetAdministratorDetails(int id)
        {
            return _votingSystemDAO.GetAdministratorDetails(id);
        }

        public IList<User_Recording> GetAdministratorRecording()
        {
            return _votingSystemDAO.GetAdministratorRecordings();
        }

        public void EditAdministrator(User_Recording Administrator)
        {
            _votingSystemDAO.EditAdministrator(Administrator);
        }
        public void AdministratorRegister(User_Recording Administrator)
        {
            _votingSystemDAO.AdministratorRegister(Administrator);
        }

        
    }
    }

# XiaodongLI97
