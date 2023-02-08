# encap
encapsulation code
import 'dart:io';

void main() {
  var bank = HBLBank();

  bank.set_prsn_amount(10000);
  bank.set_prsn_age(40);
  bank.set_prsn_name("Ranjeet Agarwal");
  bank.set_prsn_address("defence phase");
  bank.set_prsn_email("ranjeetagarwal@gmail.com");
  bank.set_prsn_mobilenum(03335564754);
  bank.set_prsn_branch("Teen talwar karachi");
  bank.set_prsn_acno(1092003054590289);

  print("                HBL Bank   \n ");

  print('Person Name           :${bank._get_prsn_name()}');
  print('Person Age            :${bank._get_prsn_age()}');
  print('Person Mobile Number  :${bank._get_prsn_mobilenum()}');
  print("Person Account Balance:${bank._get_prsn_amount()}");
  print('Person Address        :${bank._get_prsn_address()}');
  print('Person Email          :${bank._get_prsn_email()}');
  print('Person Account No.    :${bank._get_prsn_acno()}');
  print('Person Branch Name    :${bank._get_prsn_branch()}');
}

class HBLBank {
  var _prsn_name;
  var _prsn_age;
  var _prsn_amount;
  var _prsn_mobilenum;
  var _prsn_email;
  var _prsn_address;
  var _prsn_branch;
  var _prsn_acno;

  int _get_prsn_age() {
    return _prsn_age;
  }

  int _get_prsn_amount() {
    return _prsn_amount;
  }

  String _get_prsn_name() {
    return _prsn_name;
  }

  String _get_prsn_email() {
    return _prsn_email;
  }

  String _get_prsn_address() {
    return _prsn_address;
  }

  String _get_prsn_branch() {
    return _prsn_branch;
  }

  int _get_prsn_acno() {
    return _prsn_acno;
  }

  int _get_prsn_mobilenum() {
    return _prsn_mobilenum;
  }

  void set_prsn_amount(int amount) {
    this._prsn_amount = amount;
  }

  void set_prsn_age(int age) {
    this._prsn_age = age;
  }

  void set_prsn_name(String name) {
    this._prsn_name = name;
  }

  void set_prsn_address(String address) {
    this._prsn_address = address;
  }

  void set_prsn_email(String email) {
    this._prsn_email = email;
  }

  void set_prsn_mobilenum(int mobilenum) {
    this._prsn_mobilenum = mobilenum;
  }

  void set_prsn_branch(String branch) {
    this._prsn_branch = branch;
  }

  void set_prsn_acno(int acno) {
    this._prsn_acno = acno;
  }
}
