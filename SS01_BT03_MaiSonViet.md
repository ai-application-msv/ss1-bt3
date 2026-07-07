promt: Hãy phân tích đoạn code Java dưới đây để kiểm tra xem có rủi ro logic khi amount <= 0 hay không. Nếu có, hãy chỉnh sửa lại hàm calculateVAT sao cho chỉ tính VAT khi amount > 0, còn nếu giá trị không hợp lệ (âm hoặc bằng 0) thì trả về 0 hoặc ném ngoại lệ phù hợp.



public class TaxCalculator {



&#x20;   public static double calculateVAT(double amount) {

&#x20;       if (amount <= 0) {

&#x20;           // Có thể chọn trả về 0 hoặc ném ngoại lệ tùy yêu cầu nghiệp vụ

&#x20;           return 0.0;

&#x20;           // throw new IllegalArgumentException("Amount must be greater than 0");

&#x20;       }

&#x20;       return amount \* 0.1;

&#x20;   }



}

