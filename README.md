# Basic-Formatting
//This Google Apps Script formats the header row with borders, bold text, yellow background, and applies borders and font styling to the entire sheet. You can edit this format according to your task.
//Here is the Appscript code
function ColumnFormating() {
  var ss = SpreadsheetApp.getActiveSpreadsheet().getActiveSheet();

// --------Header Formating------------ 
  ss.getRange(1,1,1,ss.getLastColumn())

  .setBorder(true, true, true, true, true, true, '#000000', SpreadsheetApp.BorderStyle.SOLID)
  .setBackground('#ffff00')
  .setFontWeight('bold')
  .setHorizontalAlignment('center');
// ---------------------------------------
  var range = ss.getRange(1, 1, ss.getLastRow(), ss.getLastColumn());

  // Set border and font family
  range.setBorder(true, true, true, true, true, true, '#000000', SpreadsheetApp.BorderStyle.SOLID)
       .setFontFamily('Georgia');

};
